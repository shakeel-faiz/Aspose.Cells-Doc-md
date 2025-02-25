﻿---
title: Trabajar con la función Resaltar de GridJs
type: docs
weight: 250
url: /es/net/aspose-cells-gridjs/highlight/
description: Este artículo describe cómo usar GridJs para resaltar texto de celda, rangos de celdas, formas e imágenes.
keywords: highlight, highlight spreadsheet
---
# Trabajar con la función Resaltar de GridJs
 Admitimos las siguientes API de JS para la función Resaltar


- Habilite el resaltado y establezca el estilo de resaltado, todas las API de resaltado tendrán efecto solo después de configurar el estilo de resaltado
```javascript
xs.showHighlights(style)
 // the parameter is:
 style: the style for highlight ,currently only support color
 for example: {'color':'rgba(85, 57, 47, 0.08)'}
```

- Deshabilitar resaltado
```javascript
xs.hideHighlights()
```
- Agregar texto de celda para resaltar
```javascript
xs.sheet.addHighlightText(row,col,startpostion,endposition)
    // the parameters are:
    row:row index 
	col:column index
	startpostion: highlight start postion in cell text 
	endpostion: highlight end postion in cell text 
```

- Eliminar resaltado para texto de celda en matriz
```javascript
xs.sheet.removeHighlightText(row,col)
    // the parameters are:
    row:row index 
	col:column index
```

-  Obtenga una matriz para resaltar el texto de la celda
```javascript
xs.sheet.getHighlightTexts()
```

- Agregar rango de celdas para resaltar
```javascript
xs.sheet.addHighlightRange(sri,sci,eri,eci)
    // the parameters are:
    sri:start row index of cell range
	sci:start column index of cell range
	 eri:end row index of cell range
	eci:end column index of cell range
```

- Eliminar resaltado para rango de celdas en matriz
```javascript
xs.sheet.removeHighlightRange(sri,sci,eri,eci)
     // the parameters are:
    sri:start row index of cell range
	sci:start column index of cell range
	 eri:end row index of cell range
	eci:end column index of cell range
```

-  Obtener matriz para resaltar para rango de celdas
```javascript
xs.sheet.getHighlightRanges()
```

- Establecer el rango de celdas para resaltar inverso
```javascript
xs.sheet.setHighlightInverseRange(sri,sci,eri,eci)
    // the parameters are:
    sri:start row index of cell range
	sci:start column index of cell range
	 eri:end row index of cell range
	eci:end column index of cell range
```

- Eliminar resaltado para resaltado inverso
```javascript
xs.sheet.removeHighlightInverseRange()
     
```

-  Obtener rango de celdas de resaltado inverso
```javascript
xs.sheet.getHighlightInverseRange()
```


- Agregar forma para resaltar la matriz
```javascript
xs.sheet.addHighlightShape(shapeid)
    // the parameters are:
    shapeid: the id of shape, can be find in xs.sheet.data.shapes
```

- Eliminar forma de resaltado en matriz
```javascript
xs.sheet.removeHighlightShape(shapeid)
     // the parameters are:
    shapeid: the id of shape, can be find in xs.sheet.data.shapes
```

-  Obtener matriz para resaltar la forma
```javascript
xs.sheet.getHighlightShaps()
```


- Agregar imagen para resaltar la matriz
```javascript
xs.sheet.addHighlightImage(imageid)
    // the parameters are:
    imageid: the id of image, can be find in xs.sheet.data.images
```

- Eliminar imagen resaltada en matriz
```javascript
xs.sheet.removeHighlightImage(imageid)
     // the parameters are:
    imageid: the id of image, can be find in xs.sheet.data.images
```

-  Obtener matriz para la imagen destacada
```javascript
xs.sheet.getHighlightImages()
```

-  establecer si desea resaltar todas las hojas de trabajo, incluir todas las formas e imágenes
```javascript
xs.sheet.setHighlightAll(ishighlightall,isrerender=true)
   // the parameters are:
   ishighlightall: true or false,whether to highlight all
   isrerender: true or false,whether to reRender
```


- establecer la función de resaltado de imagen personalizada
```javascript
xs.sheet.setCustomHighlightImgFunc(func)
   // the parameters are:
   func: the custom highlight image function, it shall take two parameters ,first is ishighlight,the second one is the fabric image object 
   //we use fabric js to manage image object, please refer to http://fabricjs.com/image-filters to check more info
   below is an example for the decleare function: 
   const customHighlightImage = (ishighlight, imgobj) => {
            imgobj.filters[0] = ishighlight ? new fabric.Image.filters.Sepia() : false;
            imgobj.applyFilters();
        }
    
```

Puede encontrar más en nuestra página de demostración de github https://github.com/aspose-cells/Aspose.Cells-for-.NET/blob/master/Examples_GridJs/wwwroot/xspread/index.html
