﻿---
title: 在 Ruby 中显示或隐藏选项卡
type: docs
weight: 40
url: /zh/java/display-or-hide-tabs-in-ruby/
---
## **Aspose.Cells - 显示或隐藏选项卡**
### **隐藏标签**
隐藏选项卡使用**Aspose.Cells Java 红宝石**， 称呼**显示隐藏选项卡**模块。

**红宝石代码**

{{< highlight "ruby" >}}

 data_dir = File.dirname(File.dirname(File.dirname(__FILE__))) + '/data/'

\# Instantiating a Workbook object by excel file path

workbook = Rjb::import('com.aspose.cells.Workbook').new(data_dir + 'Book1.xls')

\# Hiding the tabs of the Excel file

workbook.getSettings().setShowTabs(false)

\# Saving the modified Excel file in default (that is Excel 2003) format

workbook.save(data_dir + "output.xls")

puts "Tabs are now hidden, please check the output file."

{{< /highlight >}}
### **使选项卡可见**
使用 Workbook 类的 setSheetTabBarHidden(false) 方法使选项卡可见。

**红宝石代码**

{{< highlight "ruby" >}}

 # Displaying the tabs of the Excel file

workbook.getSettings().setSowTabs(true)

{{< /highlight >}}
## **下载运行代码**
下载**隐藏或显示或隐藏选项卡 (Aspose.Cells)**来自以下任何社交编码网站：

- [GitHub](https://github.com/aspose-cells/Aspose.Cells-for-Java/blob/master/Plugins/Aspose_Cells_Java_for_Ruby/lib/asposecellsjava/displayhidetabs.rb)
