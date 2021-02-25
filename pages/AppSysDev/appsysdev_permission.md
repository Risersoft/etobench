---
title: Permission
keywords: Permission
sidebar: appsysdev_sidebar
permalink: appsystem-developer/db-permission.html
folder: AppSysDev
hide_sidebar: false
comments: false
---

#  Notes for DB Permissions

For dbpermission framework will auto pick it up from the **MainMenuXML + Adminbehave + objPermissionRole** fields

Need to set value for **Adminbehave** in **ClientViews, ClientFrmPrn,ClientBrowse**.

*S=Require Super Admin*

*T=Require Tenant Admin*

*I=Ignore*

*A=Allow*


For **objPermissionRole** follow below steps:


**Step.1** No need to make any changes for those objects which are called directly in MainMenuXML and can left as NULL.

**Step.2** If objects are not called directly in MainMenuXML then firstly find all these objects and make a list.

**Step.3** After make a list, find all possible navigation for called these objects & pick up the parent object's keys it may be more than one.

**Step.4** These parent object's keys set in objPermissionRole for respective objects. Eg: key1, key2

**Step.5** If parent object's key is not found for the same object type then we can enter cross object type parent by specifying **viewdef.key or frp.key or bro.key**
       
	   eg: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice

