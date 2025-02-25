﻿---
title: 检索 SQL 连接数据
type: docs
weight: 20
url: /zh/java/retrieving-sql-connection-data/
---
{{% alert color="primary" %}} 

Aspose.Cells可以帮你找回SQL连接数据。这包括连接到 SQL 服务器所需的所有数据，例如，**服务器网址**, **用户名**, **表名**, **完整的 SQL 查询**, **查询类型**, **桌子的位置**， 和**命名范围的名称**与之相关。

{{% /alert %}} 

在 Microsoft Excel 中，通过以下方式连接到数据库：

1. 点击**数据**菜单和选择**来自其他来源**其次是**从 SQL Server**.
1. 然后选择**数据**其次是**连接**.
1. 使用连接向导连接到数据库并创建数据库查询。

**在 Microsoft Excel 中显示 SQL 连接选项** 

![待办事项：图片_替代_文本](retrieving-sql-connection-data_1.png)

Aspose.Cells 提供了用于检索外部连接的 Workbook.getDataConnections() 方法。它返回工作簿中的 ExternalConnection 对象的集合。

如果 ExternalConnection 对象包含 SQL 连接数据，则可以将其类型转换为 DBConnection 对象，其属性用于检索数据库命令、命令类型、连接描述、连接信息、凭据等。







{{< gist "aspose-cells-gists" "5876dc77e47649b66bdb5deefb4b5639" "Examples-src-main-java-com-aspose-cells-examples-articles-RetrieveSQLConnectionData-RetrieveSQLConnectionData.java" >}}






