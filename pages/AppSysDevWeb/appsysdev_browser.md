---
title: Browser
keywords: Browser
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/browser.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---

# Browser

## Create

There are two options to create browser:

1.	New -> New Browser

2.	AppSystem -> Browser ->Right Click ->Copy Browser

After choosing any one option, the browser form will appear.

![](/images/browseroptionstabweb.png)

>Browser Options Tab

**Browser Key** ->User can set browser key in this block ,Entered Key should be unique for publisher and product.

    E.g. gst.Invoice

**Browser Name** ->User can set Browser Name in this block.

    E.g. Invoice

**Applications** ->User can set application name after select product in this block.

    E.g. Kasp

**Startup Node** ->User can set startup node for browser.

    E.g. ID1

**Expand Level** ->User can set expand level in this block.

    E.g. 0

**Product** ->User can select product in this block.

    E.g. ASP

**Adminbehave** -> Need to set value of Adminbehave for accessibility as per below:

*S=Require Super Admin*

*T=Require Tenant Admin*

*I=Ignore*

*A=Allow*

**Object Permission Role** -> No need to make any changes for those objects which are called directly in MainMenuXML and If objects are not called directly in MainMenuXML then find all possible navigation for called these objects & set  the parent object's keys with , if found more than one. We can enter cross object type parent by specifying *viewdef.key or frp.key or bro.key*
 
    e.g: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice



>Browser Definition Tab

![](/images/browserdefinitiontabweb.jpg)

**&lt;ROOT>**->Starting Tag Browse definition.

**&lt;ID>BROWSEID&lt;/ID>** ->User can define browse ID in this block

**&lt;DISPGRID>** -> Starting Tag for grid display.

**&lt;VIEW KEY** ->starting tag for view key assign

**&lt;DISPGRID>** -> Ending Tag for grid display.

**&lt;TREE>** -> Starting Tag for Browse tree

**<_DT KEY** -> User can set sql query for data source.

**&lt;_SET>**: This tag used to define variable for store data locally.

**<NODE KEY** ->Starting Tag for Add Node.

**NODE PARENT:** Using this we can set parent id for to be added node.

**KEY:**Using this we can set key for to be added node.

**CAPTION:**Using this tag we can set caption for added node.

**&lt;VIEW KEY**->User can assign view key in this block.

**&lt;FILTER KEY** ->User can set filter key.					

**&lt;VALUE VALUE1**->Assign filter value.				

**&lt;/FILTER>** ->Ending tag for Filter Key.

**&lt;/VIEW>** ->Ending tag for View.

**&lt;/NODE>** ->Ending tag for Node.

**&lt;/TREE>** -> Ending Tag for Browse tree.

**&lt;/ROOT>** -> Ending Tag Browse definition.

**Output:**

![](/images/BrowserDefinitionFormoutput.png)


>DataXML Tab


**SysEntXML** -> 

We set IdField for Call the Browse.

   E.g: SysID =”CustomerID”/>

![](/images/SysEntXMLWeb.jpg)



**IDSecXML** ->

*COLKEY*: Using this tag we can set table name for grid condition.

   E.g: COL KEY =”PartyType”
   
And assign uale for it like this.

   E.g: VALUE VALUE1=”C”


![](/images/IDSecXMLWeb.jpg)

**GridCondition** ->

Using this tag we can set grid condition for browser.

   E.g: <COL KEY =”SalesOrderID”/>


![](/images/GridConditionWeb.jpg)

>Children Tab

Click on **Add New** button. 

![](/images/childrentabweb.png)

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

     E.g: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice

## List

Click on **AppSystem -> Browsers**

![](/images/browserslistweb.png)

## Edit

Click on **AppSystem -> Browsers->Edit Browser**

![](/images/editbrowserweb.png)
