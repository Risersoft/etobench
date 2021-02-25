---
title: Browser
keywords: Browser
sidebar: appsysdev_sidebar
permalink: appsystem-developer/browser.html
folder: AppSysDev
hide_sidebar: false
comments: false
---

# Browser

## Create

There are two options to create browser:
1.	New -> New Browser
2.	AppSystem -> Browser ->Right Click ->Copy Browser

After choosing any one option, the browser form will appear.

![](/images/browseroptionstab.png)

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

**objPermissionRole** -> No need to make any changes for those objects which are called directly in MainMenuXML and If objects are not called directly in MainMenuXML then find all possible navigation for called these objects & set  the parent object's keys with , if found more than one. We can enter cross object type parent by specifying *viewdef.key or frp.key or bro.key*
 
    e.g: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice



>Browser Definition Tab

![](/images/browserdefinitiontab.jpg)

**&lt;ROOT>**->Starting Tag Browse definition.

**&lt;ID>BROWSEID&lt;/ID>** ->User can define browse ID in this block

**&lt;DISPGRID>** -> Starting Tag for grid display.

**&lt;VIEW KEY** ->starting tag for view key assign

**&lt;DISPGRID>** -> Ending Tag for grid display.

**&lt;TREE>** -> Starting Tag for Browse tree

**<_DT KEY** -> User can set sql query for data source.

**<NODE KEY** ->Starting Tag for Add Node.

**&lt;VIEW KEY**->User can assign view key in this block.

**&lt;IDX VALUE**->User can pass IDX value.

**&lt;FILTER KEY** ->User can set filter key.					

**&lt;VALUE VALUE1**->Assign filter value.				

**&lt;/FILTER>** ->Ending tag for Filter Key.

**&lt;/VIEW>** ->Ending tag for View.

**&lt;/NODE>** ->Ending tag for Node.

**&lt;/TREE>** -> Ending Tag for Browse tree.

**&lt;/ROOT>** -> Ending Tag Browse definition.

>DataXML Tab


**SysEntXML** -> _>

![](/images/SysEntXML.jpg)

**IDSecXML** ->

![](/images/IDSecXML.jpg)

**GridCondition** ->

![](/images/GridCondition.jpg)

>Children Tab

![](/images/childrentab.png)

## List

Click on AppSystem -> Browsers

![](/images/browserslist.jpg)

## Edit

Click on AppSystem -> Browsers->Edit Browser

![](/images/editbrowser.jpg)
