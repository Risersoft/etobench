---
title: Reports
keywords: Reports
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/views-reports.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---

# Reports

![](/images/reportweb.png)

**Max Font Size** -> User can set font size of printing output.

**Filter for Printing** -> User can set filter which apply only when printing output.

**Hide Columns**-> User cat set columns which are not require for printing.

**Print Vertical Grid Lines** -> Default value is null.

**SERIAL** -> Set true if require serial number on MMR output.

**DETAILHTFACT** -> Set row height for MMR output.

**HEADER PREFIX** -> Set Header of MMR output.

**EVAL** -> Set Evaluate value like date

**FORMAT**-> Set for mat of evaluate value.

**GROUP FIELD** -> Set Field name on which output should be group by.

**TYPE**-> Set type of group by

**< /MMR>** ->Ending Tag.



**MMRXML**->User can define format for printing known as MMRXML.

**MMR** -> < MMR > -> Starting Tag and < /MMR> -> Ending Tag.

**CAPTION** -> Using this tag we can set caption for MMR.

![](/images/MMRXMLweb.png)

![](/images/MMRXMLPrintweb.png)

**SERIAL** ->Using this tag we can set true for showing serial number for rows.

![](/images/MMRXMLSerialweb.png)

Output ->

![](/images/MMRXMLSerialOutputweb.png)

**HIDECOLS** -> Using this tag we can hide visible columns as per require.

![](/images/MMRXMLHidecolsweb.png)

![](/images/MMRXMLHidecolsinvoiceweb.png)

Output ->

![](/images/MMRXMLHidecolsoutputweb.png)

**DETAILHTFACT**->Using this tag we can set row height value.

![](/images/MMRXMLDetailhtfactweb.png)

Output ->

![](/images/MMRXMLDetailhtfactoutputweb.png)

**HEADER PREFIX**->We can set prefix for display using this tag.

![](/images/MMRXMLHeaderPrefixweb.png)

Output ->

![](/images/MMRXMLHeaderPrefixoutputweb.png)

**GROUP FIELD** ->We can set column for grouping using this tag.

![](/images/MMRXMLGroupfieldweb.jpg)

**TYPE-1**: Using this type of group we can set column for display records as per give column in Group Field and values of this column display right align.

**TYPE-2**: If we want left align for group field then we can use this.

**TYPE-3**: If we want to page break for display records of group field  then we can use this.

Output ->

![](/images/MMRXMLGroupfieldOutputweb.png)


**ALIGN** -> We use this tag for align.

![](/images/MMRXMLAlignweb.png)

**SUMM FIELD** -> We set column name for showing total.

![](/images/MMRXMLSummFieldweb.png)

Output ->

![](/images/MMRXMLSummFieldOutputweb.png)

**FOOTER PREFIX** -> We can set text to display on footer using this tag.

![](/images/MMRXMLFooterPrefixweb.png)

Output ->

![](/images/MMRXMLFooterPrefixOutputweb.jpg)




