---
title: Views
keywords: Views
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/views.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---

# Views

## Create

There are two options to create views:

1. **New -> New View**

2. **AppSystem -> Views->Right Click ->Copy View..**

After choosing any one option, the View form will appear.

![](/images/createviewweb.png)

**View Key** ->User can assign view key it is should be unique for Publisher and Product.

    E.g-ListAdvdemSaleOrder
	
![](/images/viewkeyweb.png)	

**StrView** ->User can set display name for view.

    E.g-Sales Orders
	
![](/images/strviewweb.png)	
	
**Adminbehave** ->Need to set value of Adminbehave for accessibility as per below :

*S=Require Super Admin*

*T=Require Tenant Admin*

*I=Ignore*

*A=Allow*

**Product** -> Firstly select product in which views to be created.

    E.g- ASP

![](/images/viewproduct.jpg)


**UseIDX** -> We can used IDX and check output of select SQL by giving idx value in UseIDX column.

![](/images/fixedwhere.png)

![](/images/useridx.png)

**Object Permission Role** -> No need to make any changes for those objects which are called directly in MainMenuXML and If objects are not called directly in MainMenuXML then find all possible navigation for called these objects & set  the parent object's keys with , if found more than one. We can enter cross object type parent by specifying *viewdef.key or frp.key or bro.key*

     E.g: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice
	 
	 
**Applications** ->  After select product than select applications.

    E.g-advdem

![](/images/viewapplicationsweb.png)

**Visualization Small** -> User can select grid visualization small for Mobile’s View output.

![](/images/viewvisualizationsmallweb.png)

**Grid**->                          **Chart**->

![](/images/viewgridchartweb.png)




**Dash**->     **List**->                   

![](/images/viewdashlistweb.png)

**Visualizations** ->User can select grid visualization for View output.

![](/images/viewvisualizationsweb.png)

**Grid**->

![](/images/viewgridweb.png)

**Chart**->

![](/images/viewchartweb.png)

**Dash**->

![](/images/viewdashweb.png)

**HTML**->

![](/images/viewhtml.jpg)


>DataSource Tab

User can set data source SQL for view output in this section.

![](/images/viewdatasourcetabweb.png)

**AppliFilters** ->User can set list of filters which are applicable on this view.

    E.g- Comp,Campus ..etc
	
![](/images/viewapplifiltersweb.png)

**Type** ->User can set Data source query type Default value is Fields but user can it to Template as per requirement.

![](/images/viewtypeweb.png)

**View Width Percent** ->User can set view’s output percentage.

    E.g-140.00

**Ignore Paging** ->Default value for this is False but user can set True if paging require on view output.

![](/images/viewignorepagingweb.png)

>Fields Tab

![](/images/viewfieldstabweb.png)

**Select**-> User can set fields of Data source Query without select and Form keywords.

![](/images/viewselectweb.png)

**From**-> User can set Data Source Tables or Functions.

![](/images/viewfromweb.png)

**Client**-> User can use Client if DataSoursce is PDCClientView

![](/images/viewclientweb.png)

**Group By**-> User can set Group by Fields of select query.

![](/images/viewgroupbyweb.png)

**Having**-> If SQL query included Having Condition then user can set having condition in this section.

![](/images/viewhavingweb.png)

**Order BY**-> User can set Order columns in this section.

![](/images/vieworderbyweb.png)

**Fixed Where**-> User can set fixed where conditions in this section.

![](/images/viewfixedwhereweb.png)

**ObjPermission**-> User can set Object which must be present in that Product.



>Parameters Tab


**FiltParam**-> User can set fixed filter with default value in this block.

**Note**: FiltParam should be in XML Code and use correct Syntax. If syntax not correct then errors showing in Errors block and applied Filters should be present in AppliFilters List.

    E.g.

![](/images/FiltParamweb.png)

**&lt;FILTER>** ->Starting Tag.

**FILTER KEY**->Set Filter key define in Table ClientFilter

**ACTION**->Set Default

**VALUE VALUE1**->Set IdField like FinyearID.Function Currfinid pick current finyearid.

**OPERTYPE**->Set operation type like eq for Equal.

**&lt;/FILTER>** ->Ending Tag.

*Output*->

![](/images/filtoutputweb.png)

**WhereParam** ->User can create Owen where conditions as per requirement and apply particular on menu’s in menu definition.

![](/images/WhereParamweb.png)

    E.g. Use WhereParam conditions in MenuDefination

![](/images/WhereParaminmenudifinationweb.png)

**TransformBefore**-> TransformBefore worked before view output generated.

![](/images/TransformBeforeweb.png)

    E.g. View Output before transformation.

![](/images/gridoutput.png)

![](/images/parametersoutput.jpg)

**TARGET**-> we  can set 0 in this tag.

**IDFIELD**->Assigned key field. Like Returnperiod

**PIVOT**->Assigned field to transform as header. Like SectionName

**AGGCOL**->Assigned field to transform below header respective SectionName. Like Amount

_View Output before transformation_:

![](/images/gridsummaryoutputweb.png)

**TransformAfter**-> TransformAfter worked after view output generate.

_View Output before transformation_ ->

![](/images/TransformAfterweb.png)

**ADDCOL** ->Column name which is to be added.

**KEY**->Assigned Caption name for added Field like perInc

**FORMULA**->Set value for Added column.

![](/images/formulaweb.png)

_View Output after transformation_ ->

![](/images/formulaviewweb.png)

>Common Tab

**ConditionXML**->

User can set print layout as per view output known as MMR.it is define in XML and follow below syntax.

![](/images/ConditionXMLweb.png)

*Output*:

![](/images/ConditionXMLoutputweb.png)

![](/images/ConditionXMLoutputweb1.png)


**FormatXML** -> User can format of columns of visible column like Caption, Date format etc.

![](/images/FormatXMLweb.png)

*COL KEY*: we can set database name using this tag.

    E.g: COLKEY="ProductNumber"
	
*CAPTION*:  we can set caption for display for database column name.

    E.g: CAPTION="Product No."


*Output*:

![](/images/formatxmloutputweb.png)

**Print**->


**Print Vertical Grid Lines** ->Default value is null.

**Max Font Size** ->User can set font size of printing output.

**Filter for Printing** ->User can set filter which apply only when printing output.

**Hide Columns**->User cat set columns which are not require for printing.



**MMRXML**->User can define format for printing known as MMRXML.

    E.g.

![](/images/printweb.png)

**&lt;MMR>**->Starting Tag

**SERIAL** ->Set true if require serial number on MMR output.

**DETAILHTFACT **->Set row height for MMR output.

**HEADER PREFIX **->Set Header of MMR output.

**EVAL** ->Set Evaluate value like date

**FORMAT**->Set for mat of evaluate value.

**GROUP FIELD** ->Set Field name on which output should be group by.

**TYPE**->Set type of group by

**&lt;/MMR>** ->Ending Tag.

**Output**:

![](/images/MMRoutputweb.png)

>Grid Tab

**Complex** -> User can link multiple views through a key field in this section.

![](/images/complexweb.png)

*DISPGRID* -> We can set display grid between < DISPGRID>starting & < DISPGRID> ending tags.
 
     e.g: < DISPGRID> 
          < VIEW KEY="ViewStore"/>  
          < /DISPGRID>
		  
*MAINGRID* -> we can define main grid using < MAINGRID >starting & < MAINGRID > ending tags.

     e.g: < MAINGRID>    
          < VIEW KEY="ListAdvdemStore">    
          < /MAINGRID>
		  
*VIEW KEY* -> User can set view for display grid.

     e.g: < VIEW KEY="ListAdvdemStore">
	 
*MODROW* ->We can applied user define conditions like where condition, hidecolums etc

     e.g: < MODROW>    
          < SQLWHERE2>BusinessEntityID= %idx% < /SQLWHERE2>  
          < HIDECOLS>Name< /HIDECOLS>
          < /MODROW>
		  
*SQLWHERE2*-> we can applied where condition between < SQLWHERE> & < /SQLWHERE>

     e.g :< MODROW>    
          < SQLWHERE2>BusinessEntityID= %idx% < /SQLWHERE2>  
          < /MODROW>


*HIDECOLS* ->We can hide columns using < HIDECOLS> & < /HIDECOLS>.

     e.g :< MODROW>    	
          < HIDECOLS>Name< /HIDECOLS>
          < /MODROW>
		  
*MAKEREL INSERTAT* ->set default value 0.

*BANDS* ->User can combine all child’s view in this section.
 
*FIELD* ->Set idfield 
 
*CHILD* ->Set child using give value 1, 2 etc.

Output:

![](/images/complexchild.png)

>Layout

User can define view layout in this section.

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

>Summary

User can define summary totals for views in this block

![](/images/definesummaryweb.png)

**< SUMARY COL KEY >**-> Using this tag we can set db column name which total is required.

**KEY** : Set total key word Totbal.

**FORMAT**: we can set format for required total values.

**TYPE**: In this tag we can set SUM.


**Output** ->

![](/images/summaryoutputweb.png)

>Chart Tab

**ChartXML**->

![](/images/chartxmlweb.jpg)

< clsChartModel>  is starting Tag & < /clsChartModel>  is ending tag of chart definition.

**< Legend>  & < /Legend>** : We can define orientation & position between starting & ending tag of Legend.

   E.g
   
 < Legend>        
 < Orientation>Auto< /Orientation>   
 < Position>None< /Position>    
 < Title />    
 < /Legend>
 
**< ChartType>**: We can set chart type of charts like Column,LineSymbols,Pie,Area between < ChartType>  & < /ChartType> 

**< Series>**: We can define multiple series for showing data grid between < Series> & < /Series>.
       
  Like this:
  
 < Series>      
 < clsSeriesModel> 
 < ChartType>column< /ChartType>      
 < Binding>Empcount< /Binding>          
 < BindingX>GroupName< /BindingX>     
 < /clsSeriesModel>      
 < /Series>   
**<clsSeriesModel>**: We can define layout of chart’s series between < clsSeriesModel> & < /clsSeriesModel>
 
**<Binding>**: We can set column’s name which values we want to show horizontally or respect of Y axis.

**<BindingX>**: We can set column’s name which values we want to show vertically or respect of X axis.


*Output*:

![](/images/chartxmloutputweb.png)


>Dashboard Tab

**HTML**->

![](/images/htmlweb.png)

*Output*:

![](/images/htmloutputweb.png)


**DashBoardXML**->

![](/images/DashBoardXMLweb.png)

**<DASHBOARD>**: < DASHBOARD> is starting tag & < /DASHBOARD>  is ending tag.

**How to define a Panel**: we can define a panel for dashboard using below code.

  < CONTENT>   
  < PANEL>     
  < VIEW KEY="chtAdvdemDepvsEmp">< /VIEW>    
  < /PANEL>   
  < /CONTENT>  
  
**How to define Layout of dashboard**:

  < LAYOUT>    
  < ROW>     
  < COLUMN CSSCLASS="col-md-12">    
  < ROW>       
  < COLUMN PANEL="0"  CSSCLASS="col-md-6"/>    
  < COLUMN PANEL="1"  CSSCLASS="col-md-6"/>      
  < /ROW>      
  < ROW>    
  < COLUMN PANEL="2"  CSSCLASS="col-md-6"/>       
  < COLUMN PANEL="3"  CSSCLASS="col-md-6"/>     
  < /ROW>     
  < /COLUMN>    
  < /ROW>   
  < /LAYOUT>


*Output*:

![](/images/DashBoardXMLOutputweb.png)

>Totals Tab

**TotalsXML**->

![](/images/TotalsXMLweb.png)

**< TOTAL>** is starting tag and < /TOTAL> is ending tag.

**< TITLE>**: we can set title for display.

**< FIELD>** is starting tag and </FIELD> is ending tag.

**< KEY>**: We set column for which total required like this.
 
   E.g: KEY=”Taxval”

**< SUM>**: We can use sum key word for calculate sum value of set column.

   E.g: SUM=”SUM”


*Output* ->

![](/images/totalsxmloutputweb.png)

>List Tab

User can define mobile views output in this block.

![](/images/listtabweb.png)

*Config*: We can define all list view xml code between < Config> & < /Config>

     E.g.:
	 
![](/images/listtabconfigweb.png)

*Headline*: We can define heading using < Headline> & < /Headline>.

     E.g.:
	
![](/images/listtabheadweb.png)

*Template*: we can set caption, formatting for passed arguments with position values starting 0 like {0}, {1}, {2}…etc.

     E.g.:
	 
![](/images/listtabtempweb.png)

*Arguments*: we can pass database columns as arguments like this.

     E.g.:
	 
![](/images/listtabargweb.png)

*Secondline*: we can set sub heading using < Secondline> & < / Secondline> tags.

     E.g.:

![](/images/listtabscdweb.png)

*Summary*: We can set details for summary using < summary> & < /summary> tags.

     E.g.:
	 
![](/images/listtabsumweb.png)

We can merge all details in a single line using | key words like this.

     E.g.:

![](/images/listtabsummweb.png)

*Punchtext*: we can set index or any special text parallel of main Headline using < Punchtext> & < Punchtext> tags.

     E.g.:
	 
![](/images/listtabpunchweb.png)	 
	 

*Output* ->

![](/images/listtaboutputweb.png)

>Children Tab

Click on **Add New** button. 


![](/images/viewchildrentabweb.png)

**1. Product**->User can set Products for accessibility of systableid.

     E.g. Adventure Demo

**2. AppList**->User can set applist here.

     E.g. adm

 **3. Adminbehave** -> Need to set value of Adminbehave for accessibility as per below:

*S=Require Super Admin*

*T=Require Tenant Admin*

*I=Ignore*

*A=Allow*

**4. Object Permission Role** -> No need to make any changes for those objects which are called directly in MainMenuXML and If objects are not called directly in MainMenuXML then find all possible navigation for called these objects & set  the parent object's keys with , if found more than one. We can enter cross object type parent by specifying *viewdef.key or frp.key or bro.key*

         e.g: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice

## List

Click on AppSystem -> Applications->Views

![](/images/viewlistweb.png)


## Edit

Click on AppSystem -> Applications->Right Click->Edit In View Designer

![](/images/editviewweb.png)
