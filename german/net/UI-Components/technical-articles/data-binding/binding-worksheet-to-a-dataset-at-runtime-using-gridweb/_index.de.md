﻿---
title: Binden des Arbeitsblatts an ein DataSet zur Laufzeit mit GridWeb
type: docs
weight: 70
url: /de/net/binding-worksheet-to-a-dataset-at-runtime-using-gridweb/
---
## **Mögliche Nutzungsszenarien**
Aspose.Cells.GridWeb bietet ein einfaches API, das verwendet werden kann, um ein DataSet dynamisch an ein Arbeitsblatt zu binden.
## **Binden eines Arbeitsblatts an DataSet**
Der folgende Beispielcode erläutert, wie ein Arbeitsblatt zur Laufzeit an ein DataSet gebunden wird.
## **Beispielcode**
{{< highlight "java" >}}

 // Implementing Page_Load event handler

public partial class GridBind : System.Web.UI.Page

{

    protected void Page_Load(object sender, EventArgs e)

    {

        if (Page.IsPostBack == false && this.GridWeb1.IsPostBack == false)

        {

            // Create Product Data Table

            DataTable prodTbl = new DataTable("Products");

            prodTbl.Columns.Add("ProductID");

            prodTbl.Columns.Add("ProductName");

            prodTbl.Columns.Add("ProductPrice");

            // Add products inside the data table

            prodTbl.Rows.Add(1, "Grape Juice", "$30.00");

            prodTbl.Rows.Add(3, "Mineral Water", "$25.00");

            prodTbl.Rows.Add(6, "Olive Oil", "$50.00");

            prodTbl.Rows.Add(4, "Chocolate", "$10.00");

            prodTbl.Rows.Add(7, "Oranges", "$28.00");

            // Create a DataSet and put both table in it.

            DataSet set = new DataSet();

            set.Tables.Add(prodTbl);

            // Accessing a desired worksheet

            GridWorksheet sheet = GridWeb1.WorkSheets[0];

            // Specifying Data Source for the worksheet

            sheet.DataSource = set;

            // Specifying Products tables as the DataMember

            sheet.DataMember = "Products";

            // Creating data bound columns automatically

            sheet.CreateAutoGenratedColumns();

            // Binding worksheet with DataSet

            sheet.DataBind();

        }

    }

}

{{< /highlight >}}
## **Screenshot ausgeben**
Der folgende Screenshot zeigt das GridWeb nach der Ausführung des obigen Beispielcodes.

![todo: Bild_alt_Text](binding-worksheet-to-a-dataset-at-runtime-using-gridweb_1.png)
