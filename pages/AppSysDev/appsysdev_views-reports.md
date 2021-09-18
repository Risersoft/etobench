---
title: Reports
keywords: Reports
sidebar: appsysdev_sidebar
permalink: appsystem-developer/views-reports.html
folder: AppSysDev
hide_sidebar: false
comments: false
---

# Reports

![](/images/report.png)

Print Vertical Grid Lines -> Default value is null.

Max Font Size -> User can set font size of printing output.

Filter for Printing -> User can set filter which apply only when printing output.

Hide Columns-> User cat set columns which are not require for printing.

Print Vertical Grid Lines -> Default value is null.

SERIAL -> Set true if require serial number on MMR output.

DETAILHTFACT -> Set row height for MMR output.

HEADER PREFIX -> Set Header of MMR output.

EVAL -> Set Evaluate value like date

FORMAT-> Set for mat of evaluate value.

GROUP FIELD -> Set Field name on which output should be group by.

TYPE-> Set type of group by

< /MMR> ->Ending Tag.

**MMRXML**->User can define format for printing known as MMRXML.

**MMR** -> < MMR > -> Starting Tag and < /MMR> -> Ending Tag.

**CAPTION** -> Using this tag we can set caption for MMR.

![](/images/MMRXML.jpg)

![](/images/MMRXMLPrint.jpg)

**SERIAL** ->Using this tag we can set true for showing serial number for rows.

![](/images/MMRXMLSerial.jpg)

Output ->

![](/images/MMRXMLSerialOutput.jpg)

**HIDECOLS** -> Using this tag we can hide visible columns as per require.

![](/images/MMRXMLHidecols.jpg)

![](/images/MMRXMLHidecolsinvoice.jpg)

Output ->

![](/images/MMRXMLHidecolsoutput.jpg)

**DETAILHTFACT**->Using this tag we can set row height value.

![](/images/MMRXMLDetailhtfact.jpg)

Output ->

![](/images/MMRXMLDetailhtfactoutput.jpg)

**HEADER PREFIX**->We can set prefix for display using this tag.

![](/images/MMRXMLHeaderPrefix.jpg)

Output ->

![](/images/MMRXMLHeaderPrefixoutput.jpg)

**GROUP FIELD** ->We can set column for grouping using this tag.

*TYPE 1*: Using this type of group we can set column for display records as per give column in Group Field and values of this column display right align.

![](/images/MMRXMLGroupfield.jpg)

Output ->

![](/images/MMRXMLGroupfieldOutput.jpg)

*TYPE 2*: If we want left align for group field then we can use this.

![](/images/MMRXMLGroupfieldtype2.jpg)

Output ->

![](/images/MMRXMLGroupfieldtype2output.jpg)

*TYPE 3*: If we want to page break for display records of group field  then we can use this.

![](/images/MMRXMLGroupfieldtype3.jpg)

Output ->

![](/images/MMRXMLGroupfieldtype3output.jpg)

**ALIGN** -> We use this tag for align.

![](/images/MMRXMLAlign.jpg)

**SUMM FIELD** -> We set column name for showing total.

![](/images/MMRXMLSummField.jpg)

Output ->

![](/images/MMRXMLSummFieldOutput.jpg)

**FOOTER PREFIX** -> We can set text to display on footer using this tag.

![](/images/MMRXMLFooterPrefix.jpg)

Output ->

![](/images/MMRXMLFooterPrefixOutput.jpg)




