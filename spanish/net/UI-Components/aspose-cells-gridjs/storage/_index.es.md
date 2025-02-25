﻿---
title: Trabajar con el almacenamiento de GridJs
type: docs
weight: 250
url: /es/net/aspose-cells-gridjs/storage/
description: Este artículo describe el procesamiento general de Aspose.Cells.GridJs.
keywords: file cache,storage,GridJs,GridJs storage,GridJs uid,download,uniqueid
---
# Trabajar con el almacenamiento de GridJs
## el proceso general de archivo
Después de importar un archivo de hoja de cálculo en la memoria y mostrar la interfaz de usuario,

GridJs creará un archivo de caché con el uid especificado,

 con el formato de[Aspose.Cells.SaveFormat.Xlsx](https://reference.aspose.com/cells/net/aspose.cells/saveformat/ "Aspose.Cells.SaveFormat") ,

luego, después de cada operación de actualización en la interfaz de usuario,

por ejemplo, establezca el valor de celda, establezca el estilo de celda, etc. ,

El js del lado del cliente de GridJs activará la acción del controlador para realizar una operación UpdateCell.

En esta acción, se guardará de nuevo el archivo de caché desde la memoria durante el método UpdateCell.
```C#   
        // post: /GridJs/UpdateCell
        [HttpPost] 
        public ActionResult UpdateCell( )
        {
            string p = HttpContext.Request.Form["p"];
            string uid = HttpContext.Request.Form["uid"];
            GridJsWorkbook gwb = new GridJsWorkbook();
            String ret = gwb.UpdateCell(p, uid);
            return Content(ret, "text/plain", System.Text.Encoding.UTF8);
        }
```
### donde esta el directorio de cache
R. Si implementamos GridCacheForStream y establecemos GridJsWorkbook.CacheImp.
 por ejemplo, en el siguiente código podemos poner y obtener el archivo de caché de**"D:\temp"**
```C#
Config.FileCacheDirectory=@"D:\temp";
GridJsWorkbook.CacheImp=new LocalFileCache();
public class LocalFileCache  : GridCacheForStream
    {
         
        /// <summary>
        /// Implement this method to savecache,save the stream to the cache object with the key id.
        /// </summary>
        /// <param name="s">the source stream </param>
        /// <param name="uid">the key id.</param>
        public override void SaveStream(Stream s, String uid)
        {//make sure the directory exist
            String filepath = Path.Combine(Config.FileCacheDirectory, uid);
            using (FileStream fs = new FileStream(filepath, FileMode.Create)) 
            {
                s.Position = 0;
                s.CopyTo(fs);
            }

        }

        /// <summary>
        /// Implement this method to loadcache with the key uid,return the stream from the cache object.
        /// </summary>
        /// <param name="uid">the key id</param>
        /// <returns>the stream from  the cache</returns>
        public override Stream LoadStream(String uid)
        {//make sure the directory is exist
            String filepath = Path.Combine(Config.FileCacheDirectory, uid);;
            FileStream fs = new FileStream(filepath, FileMode.Open);
            return fs;
        }
		...
```
B.Si no configuramos GridJsWorkbook.CacheImp,

 GridJs creará y guardará un archivo dentro del**Config.FileCacheDirectory** , que es el directorio de caché predeterminado que podemos configurar.

### cómo obtener el archivo de resultados actualizado
#### 1. un uid especificado para el archivo
 Asegúrese de que exista una correspondencia de mapa específica entre el archivo y el uid,

siempre puede obtener el mismo uid para un nombre de archivo específico, no de una generación aleatoria.

Por ejemplo, solo use el nombre de archivo está bien.
```C#
//in controller  
...
        public ActionResult Uidtml(String filename)
        {
 
            return Redirect("~/xspread/uidload.html?file=" + filename + "&uid=" +  Path.GetFileNameWithoutExtension(filename));
        }
 ...
        public ActionResult DetailFileJsonWithUid(string filename,string uid)
        {
            String file = Path.Combine(TestConfig.ListDir, filename);
            GridJsWorkbook wbj = new GridJsWorkbook();
            //check if already in cache
           StringBuilder sb= wbj.GetJsonByUid(uid, filename);
            if(sb==null)
            {
                Workbook wb = new Workbook(file);
                wbj.ImportExcelFile(uid, wb);
                sb = wbj.ExportToJsonStringBuilder(filename);
            }

            return Content(sb.ToString(), "text/plain", System.Text.Encoding.UTF8);
        }
```

#### 2. sincronización con la operación de interfaz de usuario
En realidad, para alguna operación de interfaz de usuario,

por ejemplo:

cambiar la hoja activa a otra,

cambiar la posición de la imagen,

rotar/cambiar el tamaño de la imagen, etc.

la acción UpdateCell no se activará.

Por lo tanto, si queremos obtener el archivo actualizado de la misma manera que muestra la interfaz de usuario,

necesitamos hacer una operación de combinación antes de guardar la acción para sincronizar esas operaciones de interfaz de usuario.
```javascript
//in the js
  function save() {
            if (!xs.buffer.isFinish()) {
              alert('updating is inprogress,please try later');
                return;
            }
            let datas = xs.datas;
            delete datas.history;
            delete datas.search;
            delete datas.images;
            delete datas.shapes;

        var jsondata = {
          sheetname: xs.sheet.data.name,
          actrow: xs.sheet.data.selector.ri,
          actcol: xs.sheet.data.selector.ci,
          datas: xs.getUpdateDatas(),
        };

        const data = {
          p: JSON.stringify(jsondata),
          uid: uniqueid,
        };
		....
		//go on to do ajax post to trigger controller action
```
```C#
//in controller action 
  GridJsWorkbook wb = new GridJsWorkbook();
  wb.MergeExcelFileFromJson(uid, p);
  //after merge do save to chache or to a stream or whaterver you want to save to ,here we just save to cache
  wb.SaveToXlsx(Path.Combine(Config.FileCacheDirectory, uid));
```         
#### 3. obtener el archivo del caché
por ejemplo: en la acción de descarga, puede obtenerlo del directorio de caché mediante uid.
```C#
//in controller  

        public async Task<IActionResult> DownloadfromBytes(string uid,string ext)
        {
            byte[] byteArr = await System.IO.File.ReadAllBytesAsync(Path.Combine(Config.FileCacheDirectory, uid) );
            string mimeType = "application/octet-stream";
            return new FileContentResult(byteArr, mimeType)
            {
                FileDownloadName = uid+ ext
            };
        }
```

Para obtener más información detallada, puede consultar el ejemplo aquí:
<https://github.com/aspose-cells/Aspose.Cells-for-.NET/tree/master/Examples_GridJs>
