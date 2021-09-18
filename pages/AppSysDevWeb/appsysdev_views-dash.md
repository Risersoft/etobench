---
title: Dashboard
keywords: Dashboard
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/views-dashboard.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---

# Dashboard Tab

## HTML

 Using this tag we can create html template.

![](/images/htmlweb.png)

*Output*

![](/images/htmloutputweb.png)

## DashBoardXML

![](/images/DashBoardXMLweb.png)

< DASHBOARD >: < DASHBOARD > is starting tag & < /DASHBOARD> is ending tag.

**How to define a Panel:** We can define a panel for dashboard using below code.

< CONTENT>   
< PANEL>     
< VIEW KEY="chtAdvdemDepvsEmp">< /VIEW>    
< /PANEL>   
< /CONTENT>
 
**How to define Layout of dashboard:**

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

*Output ->*

![](/images/Dashboardoutputweb.png)


## ActionBoxXML

We can manage navigation in this section.

![](/images/ActionBoxXMLweb.png)

**ClsActionBoxModel**: Starting tag < clsActionBoxModel> and ending tag < /clsActionBoxModel>

**ActionList**: we can define all action lists  starting tag < Actions> and ending between starting tag < ActionList> and ending tag </ActionList>

**Actions**: we can define all type actions betweentag < /Actions>
	
**clsActionModel**: we can define action model and all other properties between < clsActionModel> and < /clsActionModel>

**Category**: We can set category of actions between < Category> & < /Category> like addfrm, editfrm, nav etc.

**Caption**: we can give caption for added action as per requirement for this use tag like this:< Caption>Add Call< /Caption>

**Tag**: All objects keys should be define between < Tag> and < /Tag>
	
**FRM KEY**: we can set key for define action like this with required prams like this: < FRM KEY="frmCall">< PARAMS idfield="SalesCaseID" idvalue= "$idx$"/>< /FRM>

**PARAMS**: We can use different parameters as per applicable like IDField, IdValue etc

**Idfield**: we can pass column name in this parameter with “.

**IDvalue**: we can pass value for passed idfield like "$idx$".

![](/images/ActionBoxXMLOutputweb.png)



