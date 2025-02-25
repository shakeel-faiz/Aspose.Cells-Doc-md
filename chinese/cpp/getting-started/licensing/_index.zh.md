﻿---
title: 许可
type: docs
weight: 50
url: /zh/cpp/licensing/
---
## **评估版限制**
可以从 Aspose 网站的下载部分下载 Aspose.Cells for C++ 的免费评估版：<https://downloads.aspose.com/cells/cpp>.
## **使用文件或流对象申请许可证**
许可证可以从文件或流对象中加载。 Aspose.Cells for C++ 将尝试在以下位置查找许可证：

1. 显式路径。
1. 包含 Aspose.Cells.dll 的文件夹。
1. 包含调用 Aspose.Cells.dll 的程序集的文件夹。
1. 包含入口程序集（您的 .exe）的文件夹。
1. 称为 Aspose.Cells.dll 的程序集中的嵌入式资源。

设置许可证最简单的方法是将许可证文件放在与 Aspose.Cells.dll 文件相同的文件夹中，并指定文件名，不带路径，如下例所示。
### **从文件加载许可证**
申请许可证最简单的方法是将许可证文件放在与 Aspose.Cells.dll 文件相同的文件夹中，并仅指定文件名而不指定路径。

{{% alert color="primary" %}} 

当您调用 SetLicense 方法时，您传递的许可证名称应该是许可证文件的名称。例如，如果将许可证文件名更改为“Aspose.Cells.lic.xml”，则将该文件名传递给 Cells->SetLicense(…) 方法。

{{% /alert %}} 

**C++**

{{< highlight "csharp" >}}

 intrusive_ptr<License> license = new License();

license->SetLicense(new String("Aspose.Cells.lic"));

{{< /highlight >}}
### **从流对象加载许可证**
以下示例显示如何从流中加载许可证。

**C++**

{{< highlight "csharp" >}}

 intrusive_ptr<License>license = new License();

intrusive_ptr<FileStream> myStream = new FileStream(new String("Aspose.Cells.lic"), FileMode_Open);

license->SetLicense(myStream);

{{< /highlight >}}
