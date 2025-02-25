﻿---
title: lisanslama
type: docs
weight: 120
url: /tr/net/licensing/
---
{{% alert color="primary" %}}

 Aspose.Cells'in değerlendirme sürümünü kendi sitesinden kolayca indirebilirsiniz.[indirme sayfası](https://www.nuget.org/packages/Aspose.Cells) @ NuGet deposu. Değerlendirme sürümü, bileşenin lisanslı sürümüyle kesinlikle aynı yetenekleri sağlar. Ayrıca, bir lisans satın aldığınızda ve lisansı uygulamak için birkaç satır kod eklediğinizde, değerlendirme sürümü kolayca lisanslanır.

{{% /alert %}}

## **Değerlendirme Sürümü Sınırlamaları**

Aspose.Cells ürününün değerlendirme sürümü (lisans belirtilmeden) tam ürün işlevselliği sağlar, ancak bir programda 100 dosya ve değerlendirme filigranlı fazladan bir çalışma sayfası açmakla sınırlıdır.

Sınırlamalar aşağıda gösterilmiştir:

- **Açılan Dosya Sayısı** (Aspose.Cells)
Programınızı çalıştırırken Aspose.Cells kitaplığını kullanarak sadece 100 Excel dosyası açabilirsiniz. Uygulamanız bu sayıyı aşarsa bir istisna atılır.
- **Yapılandırma dosyası ayarları** (Aspose.Cells.GridWeb)
 Yapılandırma bölümüne (örn. web.config dosyasında) aşağıdaki kod satırlarını ekleyerek komut dosyası yolunu yeniden belirleyemezsiniz. acw_client dosyaları içeren bir klasördür ve Aspose.Cells.GridWeb bu klasörü dahili yapılandırmasını yönetmek için kullanır, GridWeb'in davranışını belirtmek ve diğer işlemleri ayarlamak için betik dosyaları, resim dosyaları ve diğer dosyalara sahiptir. Yapılandırma dosyası, kontrolün bazı durumlarda/senaryolarda yararlı olan katıştırılmış istemci kaynaklarını (resimler, komut dosyaları vb.) kullanmasını engellemek için kullanılır. Ayrıca, web.config dosyasındaki bu yapılandırma ayarları, kontrolün yalnızca LİSANSLI sürümü ile geçerli olacaktır.

**xml**

{{< highlight "csharp" >}}

 <appSettings>

<add key="aspose.cells.gridweb.acw_client_path" value="/acw_client/" />

<add key="aspose.cells.gridweb.force_script_path" value="true" />

</appSettings>

{{< /highlight >}}

{{% alert color="primary" %}}

Dosya Sistemi Web Sitelerinde veya MS Ajax uzantılarında vb. Aspose.Cells.GridWeb kontrolünü kullanıyorsanız, bu ayarlar bazı durumlarda / senaryolarda zorunlu olabilir.

{{% /alert %}}

Ayrıca, değerlendirme filigranı olan bir çalışma sayfası, Aspose.Cells kitaplığı kullanılarak oluşturulan excel dosyasında her zaman etkin çalışma sayfası olarak görünecektir. Yalnızca lisanslı sürümde, aktif çalışma sayfasını diğer çalışma sayfalarına ayarlayabilirsiniz. PDF çıktısında veya Aspose.Cells tarafından görüntü dosyasında, belgenin/görüntünün üstüne bir değerlendirme filigranı yapıştırılır. Değerlendirme Telif Hakkı Uyarısını (ekstra çalışma sayfası) GridWeb kontrolünde de gizleyemezsiniz, her zaman eklenecektir. (çalışma sayfası sekmelerinin sonunda) denetimde.

{{% alert color="primary" %}}

 Aspose.Cells'i değerlendirme sürümü sınırlaması olmadan test etmek istiyorsanız, ayrıca bir istekte bulunabilirsiniz.[30 Günlük Geçici Lisans](https://purchase.aspose.com/temporary-license).

{{% /alert %}}

## **Aspose.Cells Bileşeninde Lisans Uygulama**

Lisans, ürün adı, lisanslandığı geliştirici sayısı, abonelik bitiş tarihi gibi ayrıntıları içeren düz metin bir XML dosyasıdır. Dosya dijital olarak imzalanmıştır, bu nedenle dosyayı değiştirmeyin. Dosyaya yanlışlıkla fazladan bir satır eklenmesi bile onu geçersiz kılacaktır. Değerlendirme sınırlamasını önlemek istiyorsanız, Aspose.Cells'i kullanmadan önce bir lisans ayarlamanız gerekir. Uygulama (veya süreç) başına yalnızca bir kez lisans ayarlamak gerekir. Lisans bir dosyadan, akıştan veya gömülü bir kaynaktan yüklenebilir.

Aspose.Cells lisansı aşağıdaki konumlarda bulmaya çalışır:

- açık yol
- Aspose.Cells.dll dosyasının bulunduğu klasör
- Aspose.Cells.dll adlı derlemeyi içeren klasör
- Giriş derlemesini içeren klasör (.exe'niz)
- Derlemede Aspose.Cells.dll olarak adlandırılan katıştırılmış bir kaynak

Bir lisansı dosyadan veya akıştan veya katıştırılmış bir kaynaktan uygulamak için iki yaygın yöntem vardır.

### **Diskten veya Akıştan Lisans Uygulama**

Bir lisans ayarlamanın en kolay yolu, lisans dosyasını Aspose.Cells.dll ile aynı klasöre koymak ve yolu olmadan sadece dosya adını belirtmektir.

{{< highlight "csharp" >}}

 //Instantiate an instance of license and set the license file through its path

Aspose.Cells.License license = new Aspose.Cells.License();

license.SetLicense("Aspose.Cells.lic");

{{< /highlight >}}

{{% alert color="primary" %}}

 SetLicense yöntemini çağırdığınızda lisans adı, lisans dosyanızın adı ile aynı olmalıdır. Örneğin, lisans dosyası adını şu şekilde değiştirebilirsiniz:**Aspose.Cells.lic.xml**. Ardından kodunuzda değiştirilen lisans adını kullanmalısınız (**Aspose.Cells.lic.xml**) SetLicense yöntemi için.

{{% /alert %}}

Akıştan lisans yüklemek de mümkündür.

{{< highlight "csharp" >}}

 //Instantiate an instance of license and set the license through a stream

Aspose.Cells.License license = new Aspose.Cells.License();

license.SetLicense(myStream);

{{< /highlight >}}

### **Tarifeli Lisansı Uygulama**

Aspose.Cells, geliştiricilerin ölçülü anahtar uygulamasına izin verir. Yeni bir lisanslama mekanizmasıdır. Yeni lisanslama mekanizması, mevcut lisanslama yöntemiyle birlikte kullanılacaktır. API özelliğinin kullanımına göre faturalandırılmak isteyen müşterilerimiz tarifeli lisanslamayı kullanabilirler. Daha fazla ayrıntı için lütfen bkz.[Ölçülü Lisanslama SSS](https://purchase.aspose.com/faqs/licensing/metered)bölüm.

yeni bir sınıf[ölçülü](https://reference.aspose.com/cells/net/aspose.cells/metered)ölçülü anahtarı uygulamak için tanıtıldı. Ölçülü genel ve özel anahtarın nasıl ayarlanacağını gösteren örnek kod aşağıdadır.

{{< highlight "csharp" >}}

 //Set metered public and private keys

Metered metered = new Metered();

//Access the setMeteredKey property and pass public and private keys as parameters

metered.SetMeteredKey("*************", "*************");

//Instantiate a new Workbook

Workbook workbook = new Workbook();

//Check if the license is set

Console.WriteLine(workbook.IsLicensed);

//Get the Consumption quantity

decimal amountBefore = Metered.GetConsumptionQuantity();

Console.WriteLine(amountBefore);

Workbook workbook2 = new Workbook("e:\\test2\\Book1.xlsx");

workbook2.Save("e:\\test2\\out1.xlsx");

//Since uploading data is already running on another thread, so you might need to wait for some time (optional)

System.Threading.Thread.Sleep(10000);

//Get the Consumption quantity again which should be greater a bit

decimal amountAfter = Metered.GetConsumptionQuantity();

Console.WriteLine(amountAfter);

{{< /highlight >}}

### **Katıştırılmış Kaynak Kullanma**

Lisansı uygulamanızla birlikte paketlemenin ve kaybolmamasını sağlamanın başka bir zarif yolu, onu Aspose.Cells'i çağıran derlemelerden birine katıştırılmış bir kaynak olarak dahil etmektir. Lisans dosyasını katıştırılmış bir kaynak olarak dahil etmek için aşağıdaki adımları gerçekleştirin :

1.  Visual Studio .NET'de, lisans (.lic) dosyasını seçime göre projeye dahil edin**Mevcut Öğeyi Ekle** dan**Dosya** Menü.
1. Solution Explorer'da dosyayı seçin ve ayarlayın**Eylem Oluştur** ile**Gömülü Kaynak** Özellikler penceresinde

 Derlemeye gömülü lisansa (gömülü kaynak olarak) erişmek için, Microsoft .NET Çerçevesinin System.Reflection.Assembly sınıfının GetExecutingAssembly ve GetManifestResourceStream yöntemlerini çağırmak gerekli değildir. Tek yapmanız gereken, lisans dosyasını projenize gömülü bir kaynak olarak eklemek ve lisans dosyasının adını SetLicense yöntemine iletmektir. bu**Aspose.Cells.License** class, gömülü kaynaklarda lisans dosyasını otomatik olarak bulacaktır. Uygulamalarınızda bu lisans (katıştırılmış) ayarlama yöntemini anlamak için lütfen aşağıda verilen örneği inceleyin.

{{< highlight "csharp" >}}

 //Instantiate the License class

Aspose.Cells.License license = new Aspose.Cells.License();

//Pass only the name of the license file embedded in the assembly

license.SetLicense("Aspose.Cells.lic");

{{< /highlight >}}

## **Aspose.Cells Grid Kontrollerinde Lisans Ayarlama**

Aspose.Cells Grid Suite'te lisans bir dosyadan, akıştan veya gömülü bir kaynaktan yüklenebilir. Aspose.Cells.GridDesktop / Aspose.Cells.GridWeb aşağıdaki konumlarda lisansı bulmaya çalışır:

1. açık yol
1. Bileşenin dll'sini içeren klasör (Aspose.Cells.GridDesktop veya Aspose.Cells.GridWeb'de bulunur)
1. Bileşenin dll'sini çağıran derlemeyi içeren klasör (Aspose.Cells.GridDesktop veya Aspose.Cells.GridWeb'de bulunur)
1. Giriş derlemesini içeren klasör (.exe'niz)
1. Bileşenin dll'sini çağıran derlemede katıştırılmış bir kaynak (Aspose.Cells.GridDesktop veya Aspose.Cells.GridWeb'de bulunur)

{{% alert color="primary" %}}

Aspose.Cells.GridDesktop kontrolünü kullanıyorsanız, lisans sınıfı Aspose.Cells.GridDesktop.License olarak kullanılacaktır, ancak Aspose.Cells.GridWeb kontrolünü kullanıyorsanız, lisansı ayarlamak için Aspose.Cells.GridWeb.License sınıfı kullanılacaktır.

{{% /alert %}}

### **Diskten veya Akıştan Lisans Uygulama**

Bir lisans ayarlamanın en kolay yolu, lisans dosyasını bileşenin dll dosyasıyla aynı klasöre koymak (Aspose.Cells.GridWeb'de bulunur) ve yolu olmadan sadece dosya adını belirtmektir.

{{< highlight "csharp" >}}

//Instantiate an instance of license and set the license file through its path

Aspose.Cells.GridWeb.License license = new Aspose.Cells.GridWeb.License();

license.SetLicense("MyLicense.lic");

{{< /highlight >}}

{{% alert color="primary" %}}

SetLicense yöntemini çağırdığınızda, lisans adı, lisans dosya adınızla aynı olmalıdır. Örneğin, lisans dosyası adını "MyLicense.lic.xml" olarak değiştirebilirsiniz. Ardından kodunuzda, SetLicense yöntemi için değiştirilmiş lisans adını (yani MyLicense.lic.xml) kullanmalısınız.

{{% /alert %}}

Akıştan lisans yüklemek de mümkündür.

{{< highlight "csharp" >}}

//Instantiate an instance of license and set the license through a stream

Aspose.Cells.GridWeb.License license = new Aspose.Cells.GridWeb.License();

license.SetLicense(myStream);

{{< /highlight >}}

### **Bir Lisansı Gömülü Kaynak Olarak Uygulama**

Lisansı uygulamanızla birlikte paketlemenin ve kaybolmamasını sağlamanın başka bir zarif yolu, bileşenin dll'sini çağıran derlemelerden birine (Aspose.Cells.GridDesktop dahil) katıştırılmış bir kaynak olarak dahil etmektir. Lisans dosyasını katıştırılmış bir kaynak olarak dahil etmek için aşağıdaki adımları gerçekleştirin:

1.  Visual Studio .NET'de, lisans (.lic) dosyasını kullanarak projeye dahil edin.**Mevcut Öğeyi Ekle** üzerindeki seçenek**Dosya** Menü.
1. Çözüm Gezgini'nde dosyayı seçin ve Özellikler penceresinde Eylem Oluştur'u Gömülü Kaynak olarak ayarlayın.
1. Derlemede katıştırılmış lisansa (katıştırılmış kaynak olarak) erişmek için, Microsoft .NET Framework'ün System.Reflection.Assembly sınıfının GetExecutingAssembly ve GetManifestResourceStream yöntemlerini çağırmanız gerekmez. projelendirin ve lisans dosyasının adını SetLicense yöntemine iletin. Lisans sınıfı, gömülü kaynaklarda lisans dosyasını otomatik olarak bulur.

Uygulamalarınıza katıştırılmış bir kaynak olarak bir lisans uygulama yöntemini anlamak için lütfen aşağıda verilen örneği inceleyin.

{{< highlight "csharp" >}}

 //Instantiate the License class

Aspose.Cells.GridDesktop.License license = new Aspose.Cells.GridDesktop.License();

//Pass only the name of the license file embedded in the assembly

license.SetLicense("Aspose.Total.lic");

{{< /highlight >}}

## **WinForm Uygulaması için Aspose.Cells.GridDesktop'ta Lisans Uygulama**

Lisanslama kodunuzu başvurunuz başlamadan önce girmeniz ve yalnızca bir kez uygulamanız önerilir. Örneğin, bir Windows C# uygulaması için lisans kodunu Ana yönteme yerleştirin.

{{< highlight "csharp" >}}

public class Form1 : System.Windows.Forms.Form

{

private Aspose.Cells.GridDesktop.GridDesktop gridDesktop1;

/// <summary>

/// Required designer variable.

/// </summary>

private System.ComponentModel.Container components = null;

public Form1()

{

//

// Required for Windows Form Designer support

//

InitializeComponent();

//

// TODO: Add any constructor code after InitializeComponent call

//

}

/// The main entry point for the application.

/// </summary>

.

.

.

.

[STAThread]

static void Main()

{

Aspose.Cells.GridDesktop.License lic = new Aspose.Cells.GridDesktop.License();

//Use this line if you are using an explicit path for the license file.

lic.SetLicense(@"C:\MyLicense.lic");

//Or use the line below if you are using the license file as an embedded resource.

//lic.SetLicense("MyLicense.lic");

Application.Run(new Form1());

}

private void Form1_Load(object sender, System.EventArgs e)

{

Aspose.Cells.GridDesktop.Worksheet sheet = this.gridDesktop1.Worksheets.Add("MySheet");

sheet.Cells["A1"].SetCellValue("Hello");

gridDesktop1.ActiveSheetIndex = 1;

}

}

{{< /highlight >}}

## **Aspose.Cells.GridWeb'de Lisans Uygulamaya İlişkin Notlar**

Lisans kodunu web uygulamanızın Global.asax.cs dosyasına koymanız önerilir (bu lisans dosyasının " d:\ " sürücüsüne yerleştirildiği varsayılır):

{{< highlight "csharp" >}}

 protected void Application_Start(Object sender, EventArgs e)

{

    Aspose.Cells.GridWeb.License lic = new Aspose.Cells.GridWeb.License();

    lic.SetLicense(@"d:\Aspose.Cells.GridWeb.lic.xml");

}

{{< /highlight >}}

Akıştan Lisans Yükleme

{{< highlight "csharp" >}}

 protected void Application_Start(Object sender, EventArgs e)

{

    Aspose.Cells.GridWeb.License lic = new Aspose.Cells.GridWeb.License();

    lic.SetLicense(myStream);

}

{{< /highlight >}}
