---
title: Common
keywords: Common
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/views-common.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---


# Common Tab

## Transformations

**Transform Before** -> Transform before worked before view output generated.

![](/images/TransformBeforeweb.png)

**< MAINGRID >** is starting tag and **< /MainGrid>** is ending tag.

**SCROSS** -> Type of transformation. 
 
**TARGET** -> we can set index of defined complex views in view in this tag if complex view is not define then we can set 0 for this tag.

**IDFIELD**->Assigned key field. Like Returnperiod

**PIVOT**->Assigned field to transform as header. Like SectionName

**AGGCOL**->Assigned field to transform below header respective SectionName. Like Amount

*View Output before Transformation*

![](/images/gridoutputweb.png)

**TransformAfter**-> TransformAfter worked after view output generate.

*View Output before Transformation*

![](/images/TransformAfterweb.png)

**ADDCOL** ->Column name which is to be added.

**KEY**->Assigned Caption name for added Field like perInc

**FORMULA**->Set value for Added column.

![](/images/formulaweb.png)

*View Output after Transformation*

![](/images/formulaviewweb.png)

## Type of Transformations

2.1. **SCROSS:** For defining Scross we can used below xml tags.

![](/images/commontabweb.png)

**< MAINGRID> < /MAINGRID>** ->  < MainGrid> is starting tag and < /MainGrid> is ending tag.

**< SCROSS> < /SCROSS>** ->  < SCROSS> is starting tag and < /SCROSS> is ending tag.
 
**TARGET** -> We can set index of defined complex views in view in this tag if complex view is not define then we can set 0 for this tag.

**PIVOT** -> Assigned field to transform as header. Like Descrip

**IDFIELD** -> We can set unique key field for idfield. Like EmployeeID

**AGGCOL** -> We can set field to transform below header respective assigned column in pivot like Descrip. i.e Dated

![](/images/Scrossoutputweb.jpg)


2.2. **COCROSS:**

![](/images/Cocrossweb.jpg)

**< MAINGRID >  < /MAINGRID >** ->  < MainGrid > is starting tag and < /MainGrid > is ending tag.

**< COCROSS >  < /COCROSS >** ->  <COCROSS> is starting tag and </COCROSS>  is ending tag.

**IDFIELD** ->  We can set unique key field for idfield. Like EmployeeID

**COPYDT** -> we can set 0 in this tag

**PIVOT** -> Assigned field to transform as header. Like MaterialDept

**AGGCOL** -> We can set field to transform below header respective assigned column in pivot like MaterialDept. i.e IncentiveAmount

**VIEW INDEX** -> we can set 0, 1, 2 in this tag

**PREFIX** -> we can set text for display as prefix.

**COLOR** -> we can set colour for row using this tag.

![](/images/Cocrossoutputweb.jpg)

2.3. **ATTRIBUTIZE:** 

![](/images/ATTRIBUTIZEweb.jpg)

**< MAINGRID >  < /MAINGRID >** -> < MainGrid > is starting tag and < /MainGrid > is ending tag.

**< ATTRIBUTIZE >  < /ATTRIBUTIZE >** -> < ATTRIBUTIZE > is starting tag and < / ATTRIBUTIZE >  is ending tag.

**TARGET** -> we can set index of defined complex views in view in this tag if complex view is not define then we can set 0 for this tag.

**PIVOT** -> Set starting fixed latter’s of columns to transform as header and respective values are showing below of respective columns. Like Attrib1Name, Attrib1Value, Attrib2Name, Attrib2Value, Attrib3Name, Attrib3Value.

*View Output before Transformation*

![](/images/ATTRIBUTIZEOutputBeforeweb.jpg)

*View Output after Transformation*

![](/images/ATTRIBUTIZEOutputAfterweb.jpg)

2.4. **SUMMARIZE:**

![](/images/SUMMARIZEweb.jpg)

**< MAINGRID > < /MAINGRID >** ->  < MainGrid > is starting tag and < /MainGrid > is ending tag.

**< SUMMARIZE> < /SUMMARIZE >** -> < SUMMARIZE > is starting tag and </ SUMMARIZE >  is ending tag.

**TARGET** -> we can set index of defined complex views in view in this tag if complex view is not define then we can set 0 for this tag.

**SUMCOLS** -> we can set columns for sum.

**GROUPBYCOLS** -> we can set columns for group.

2.5. **SUMUPALL:**

![](/images/SUMUPALLweb.jpg)

**< TOTGRID >  < /TOTGRID >** -> < TOTGRID > is starting tag and </ TOTGRID > is ending tag.

**< SUMUPALL >  < /SUMUPALL >** -> < SUMUPALL > is starting tag and </ SUMUPALL > is ending tag.

**VIEWINDEX** -> we can set view index under this tag like 0, 1, 2 etc..
 
**AFTERCOL** -> In this tag we can set column name where we have require sum of columns.

**FORMAT** -> Using this tag we can set format as per require for summary totals.

![](/images/SUMUPALLOutputweb.jpg)



## ConditionXML

User can set print layout as per view output known as MMR.it is define in XML and follow below syntax.

![](/images/ConditionXMLweb.png)

**< CONDITION>** -> Starting Tag

**FILTER KEY** -> we can apply filter for output of MMR reports.

**VALUE VALUE1** -> Assigned values for applied filter key.

**</FILTER KEY>** -> Ending tag of filter key.

**< OVERRIDE>** -> Starting Tag  **</ OVERRIDE>**-> Ending tag 

**< MMRXML>** -> Starting Tag **< /MMRXML>** -> Ending tag

**< STRVIEW> < /STRVIEW>** -> we can set display name for view between these tags.

**< MMR>** ->Starting Tag and **< MMR>** ->Ending Tag

**HEADER PREFIX** -> Set Header of MMR output.

**EVAL** -> Set Evaluate value like date

**FORMAT** -> Set for mat of evaluate value.

**GROUP FIELD** -> Set Field name on which output should be group by.

**SUMM FIELD** -> we can set column for sum values.

**TYPE** ->Set type of group by

**</ CONDITION >** ->Ending Tag.

Output ->

![](/images/ConditionXMLOutputweb.jpg)


## FormatXML

User can format of columns of visible column like Caption, Date format etc.

![](/images/FormatXMLweb.png)

**COL KEY** -> we can set database column name in this tag.

**CAPTION** -> we can set caption of assigned column in Col Key for display.

**FORMAT** -> we can format of date type columns or other type columns as per requirement.

**Output**:

![](/images/formatxmloutputweb.png)



