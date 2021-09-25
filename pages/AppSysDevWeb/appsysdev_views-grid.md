---
title: Grid
keywords: Grid
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/views-grid.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---


# Grid Tab

## Layout


**Layout**-> User can define view layout in this section.

![](/images/layoutweb.png)

**Inverted View**->User can marked if require visibility of columns horizontally.

**Ban Sort**->User can marked in require sorting on view.

**Reverse Direction**-> User can marked if require visibility of columns from Ending.

**Column Headers**->User marked if require fixed header.

**Fix Columns**-User can set fixed no of columns in this block.

**strWidth**->User can width for visible fields in this block.

**Heading Factor**->User can set width for header in this block.

**strBand**->User can set Display name for view.

**Row Height Factor**->user can set row height in this block.

**GroupOn**->User can set Group column Name in this block.

**Default Wid Fact.**->User can set default value of column’s width.

**Allow Group By**->User can marked if allow group by on header columns.

**Sort On Columns**->User can set columns require sorting on columns.


## Complex

User can link multiple views through a key field in this section.

![](/images/complexweb.png)

DISPGRID-> We can set display grid between <DISPGRID>starting & <DISPGRID> ending tags.

    e.g: <DISPGRID> 
         <VIEW KEY="ViewStore"/>  
         </DISPGRID>
		
MAINGRID -> We can define main grid using < MAINGRID >starting & < MAINGRID > ending tags.

    e.g: <MAINGRID>    
         <VIEW KEY="ListAdvdemStore">    
         </MAINGRID>
		 
VIEW KEY -> User can set view for display grid.

    e.g: <VIEW KEY="ListAdvdemStore">
	
	
MODROW -> We can applied user define conditions like where condition, hidecolums etc.

    e.g: <MODROW>    
         <SQLWHERE2>BusinessEntityID= %idx% </SQLWHERE2>  
         <HIDECOLS>Name</HIDECOLS>
         </MODROW>
		 
SQLWHERE2-> We can applied where condition between <SQLWHERE> & </SQLWHERE>.

    e.g :< MODROW>    
         <SQLWHERE2>BusinessEntityID= %idx% </SQLWHERE2>  
         </MODROW>

HIDECOLS-> We can hide columns using <HIDECOLS> & </HIDECOLS>.

    e.g :< MODROW>    	
         <HIDECOLS>Name</HIDECOLS>
         </MODROW>
		
		
MAKEREL INSERTAT ->set default value 0.

BANDS ->User can combine all child’s view in this section.

FIELD ->Set idfield

CHILD ->Set child using give value 1, 2 etc.

*Output*

![](/images/complexoutputweb.png)

## Summary

User can define summary totals for views in this block

![](/images/definesummaryweb.png)

< SUMARY COL KEY > Using this tag we can set db column name which total is required.

*KEY:* Set total key word Totbal.

*FORMAT:* we can set format for required total values.We can also use different format specifier as per below.

![](/images/summaryformat.jpg)

*TYPE:* In this tag we can set SUM.


**Output** ->

![](/images/summaryoutputweb.png)

**TotalsXML**-> Using this tag we can set summary totals of require columns.

![](/images/TotalsXMLweb.png)

TOTAL is starting tag and < /TOTAL> is ending tag.

TITLE -> we can set title for display.

FIELD -> < FIELD>  is starting tag and < /FIELD> is ending tag.

KEY -> We set column for which total required like this.

KEY=”Taxval”

SUM-> We can use sum key word for calculate sum value of set column.

  E.g: SUM=”SUM”


**Output** ->

![](/images/totalsxmloutputweb.png)





