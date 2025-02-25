﻿---
title: Начиная
type: docs
weight: 10
url: /ru/net/getting-started/
---
{{% alert color="primary" %}} 

На этой странице показано, как установить Aspose Cells и создать приложение Hello World.

{{% /alert %}}

## **Установка**

### **Установите с Aspose.Cells по NuGet**

 NuGet — это самый простой способ загрузить и установить Aspose.Cells for .NET.

1.  Откройте Microsoft Visual Studio и диспетчер пакетов NuGet.
1.  Введите в поиске «aspose.cells» нужный номер Aspose.Cells for .NET.
1. Нажмите «Установить», Aspose.Cells for .NET будет загружен и указан в вашем проекте.
**![Установить с Aspose от Cells до NuGet](install-through-nuget.png)**

 Вы также можете загрузить его с веб-страницы nuget для aspose.cells:
[Aspose.Cells for .NET NuGet Пакет](https://www.nuget.org/packages/Aspose.Cells/)

[Больше шагов для деталей](/cells/ru/net/installation/)

### **Установите Aspose.Cells на Windows**

1. Загрузите Aspose.Cells.msi со следующей страницы:
[Скачать Aspose.Cells.msi](https://downloads.aspose.com/cells/net/)
1. Дважды щелкните msi Aspose Cells и следуйте инструкциям по его установке:

**![Установить Aspose Cells в Windows](install-on-windows.png)**

[Больше шагов для деталей](/cells/ru/net/installing-aspose-cells-on-windows/)

### **Установите Aspose.Cells на линукс**

В этом примере я использую Ubuntu, чтобы показать, как начать использовать Aspose.Cells в Linux.

1. Создайте приложение .netcore с именем «AsposeCellsTest».
2. Откройте файл "AsposeCellsTest.csproj", добавьте в него следующие строки для ссылок на пакеты Aspose.Cells:
{{< highlight "plain" >}}
  <ItemGroup>
    <PackageReference Include="Aspose.Cells" Version="22.12" />
  </ItemGroup>
{{< /highlight >}}
3. Откройте проект с помощью VSCode в Ubuntu:
**![Установить Aspose Cells в Linux](install-on-linux.png)**
4. запустите тест со следующим кодом:
{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-StartOnLinux.cs" >}}

Примечание. Aspose.Cells Для .NetStandard может поддерживать ваши требования к Linux.

Применяется к: NetStandard2.0, NetCore2.1, NetCore3.1, Net5.0, Net6.0 и расширенной версии.

### **Установите Aspose.Cells на MAC OS**

В этом примере я использую macOS High Sierra, чтобы показать, как начать использовать Aspose.Cells в MAC OS.

1. Создайте приложение .netcore с именем «AsposeCellsTest».
2. Откройте приложение с помощью Visual Studio для Mac, затем установите номера с Aspose от Cells до NuGet:
**![Установить Aspose Cells в macOS](install-on-mac-os.png)**
3. запустите тест со следующим кодом:
{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-StartOnMacOS.cs" >}}
4. Если вам нужно использовать функции, связанные с рисованием, установите libgdiplus в macOS, см.:
[Как установить libgdiplus в macOS](/cells/ru/net/how-to-install-libgdiplus-in-macos/)

Примечание: Aspose.Cells For .NetStandard может поддерживать ваши требования к MAC OS.

Применяется к: NetStandard2.0, NetCore2.1, NetCore3.1, Net5.0, Net6.0 и расширенной версии.

### **[Запустите Aspose Cells в Docker](/cells/net/how-to-run-aspose-cells-in-docker/)**

### **Как использовать графическую библиотеку на платформах, отличных от Windows, с Net6**

 Aspose.Cells для Net6 теперь использует SkiaSharp в качестве графической библиотеки, как рекомендовано в[официальное заявление от Microsoft](https://github.com/dotnet/designs/blob/f9d006073b7a019bd2021e99c66516447f7fb1a6/accepted/2021/system-drawing-win-only/system-drawing-win-only.md) . Дополнительные сведения об использовании Aspose.Cells с NET6 см.[Как запустить Aspose.Cells для .Net6](/cells/ru/net/how-to-run-aspose-cells-for-net6/).

## **Создание приложения Hello World**

Следующие шаги создают приложение Hello World, используя Aspose.Cells API:

1.  Если у вас есть лицензия, то[применить это](/cells/ru/net/licensing/).
 Если вы используете ознакомительную версию, пропустите строки кода, связанные с лицензией.
1.  Создайте экземпляр[Рабочая тетрадь](https://reference.aspose.com/cells/net/aspose.cells/workbook) class для создания нового файла Excel или открытия существующего файла Excel.
1. Получите доступ к любой нужной ячейке рабочего листа в файле Excel.
1.  Вставьте слова**Hello World!** в ячейку, к которой осуществляется доступ.
1. Создайте измененный файл Excel Microsoft.

Реализация вышеуказанных шагов продемонстрирована на примерах ниже.

### **Пример кода: создание новой книги**

В следующем примере создается новая книга с нуля, вставляется "Hello World!" в ячейку A1 на первом листе и сохраняет как файл Excel.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Introduction-FirstApplication-1.cs" >}}

### **Пример кода: открытие существующего файла**

В следующем примере открывается существующий файл шаблона Excel Microsoft «Sample.xlsx», вставляется «Hello World!» в ячейку A1 на первом листе и сохраняет как файл Excel.

{{< gist "aspose-cells-gists" "88c9872508ec3150c552eb5155edf06e" "Examples-CSharp-Introduction-OpenExistingFile-1.cs" >}}
