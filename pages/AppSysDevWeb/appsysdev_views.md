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


## List

Click on AppSystem -> Applications->Views

![](/images/viewlistweb.png)


## Edit

Click on AppSystem -> Applications->Right Click->Edit In View Designer

![](/images/editviewweb.png)
