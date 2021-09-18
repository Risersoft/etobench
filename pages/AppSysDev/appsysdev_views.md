---
title: Views
keywords: Views
sidebar: appsysdev_sidebar
permalink: appsystem-developer/views.html
folder: AppSysDev
hide_sidebar: false
comments: false
---

# Views

## Create

There are two options to create views:

1. **New -> New View**

2. **AppSystem -> Views->Right Click ->Copy View..**

After choosing any one option, the View form will appear.

![](/images/createview.png)

**Product** -> Firstly select product in which views to be created.

    E.g- ASP

![](/images/viewproduct.jpg)

**Applications** ->  After select product than select applications.

    E.g-Kasp

![](/images/viewapplications.png)

**View Key** ->User can assign view key it is should be unique for Publisher and Product.

    E.g-listInvoice

**StrView** ->User can set display name for view.

    E.g-Invoice
	
**Adminbehave** ->Need to set value of Adminbehave for accessibility as per below :

*S=Require Super Admin*

*T=Require Tenant Admin*

*I=Ignore*

*A=Allow*


**Object Permission Role** -> No need to make any changes for those objects which are called directly in MainMenuXML and If objects are not called directly in MainMenuXML then find all possible navigation for called these objects & set  the parent object's keys with , if found more than one. We can enter cross object type parent by specifying *viewdef.key or frp.key or bro.key*

     E.g: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice

**Generate** ->Using this button we can see output of select SQL clicking on Generate Button.

![](/images/generatebutton.png)

**UseIDX** -> We can used IDX and check output of select SQL by giving idx value in UseIDX column and verify output after pressed Generate button.

![](/images/fixedwhere.png)

![](/images/useridx.png)

**Visualizations** ->User can select grid visualization for View output.

![](/images/viewvisualizations.png)

**Grid**->

![](/images/viewgrid.png)

**Chart**->

![](/images/viewchart.png)

**Dash**->

![](/images/viewdash.png)

**HTML**->

![](/images/viewhtml.jpg)

**Visualization Small** -> User can select grid visualization small for Mobile’s View output.

![](/images/viewvisualizationsmall.png)

**Grid**->                          **Chart**->

![](/images/viewgridchart.jpg)




**Dash**->     **List**->                   

![](/images/viewdashlist.jpg)




## List

Click on AppSystem -> Applications->Views

![](/images/viewlist.png)


## Edit

Click on AppSystem -> Applications->Right Click->Edit In View Designer

![](/images/editview.jpg)
