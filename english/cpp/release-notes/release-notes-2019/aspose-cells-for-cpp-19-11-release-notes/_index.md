---
title: Aspose.Cells for CPP 19.11 Release Notes
type: docs
weight: 10
url: /cpp/aspose-cells-for-cpp-19-11-release-notes/
---

{{% alert color="primary" %}} 

This page contains release notes for Aspose.Cells for C++ 19.11.

{{% /alert %}} 

|**Key**|**Summary**|**Category**|
| :- | :- | :- |
|CELLSCPP-218|Support for adding some sort of Callback event/mechanism that notifies the progress of conversion (e.g Excel to PDF)|New Feature|
|CELLSCPP-220|Fix x64 debug mode crush while integrating other C++ products|New Feature|
### **Public API and Backwards Incompatible Changes**
The following is a list of any changes made to the public API such as added, renamed, removed or deprecated members as well as any non-backward compatible change made to Aspose.Cells for C++. If you have concerns about any change listed, please raise it on the Aspose.Cells support forum.

Add IPdfSaveOptions::SetIPageSavingCallback
Add IPdfSaveOptions::GetIPageSavingCallback
Add PageSavingArgs::GetPageIndex
Add PageSavingArgs::GetPageCount
Add PageStartSavingArgs::SetToOutput
Add PageStartSavingArgs::IsToOutput
Add PageEndSavingArgs::HasMorePages
Add PageEndSavingArgs::SetHasMorePages








