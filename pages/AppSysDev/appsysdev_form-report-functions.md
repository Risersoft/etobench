---
title: Form/Report/Functions
keywords: Form/Report/Functions
sidebar: appsysdev_sidebar
permalink: appsystem-developer/form-report-functions.html
folder: AppSysDev
hide_sidebar: false
comments: false
---


# Form/Report/Functions

## Create

There are two options to create form/report/functions:
1.	New -> New Form/Report/Functions
2.	AppSystem -> Form/Report/Functions ->Right Click ->Copy Form/Report/Functions

After choosing any one option, the Form/Report/Functions form will appear.  

![](/images/form-report-function.jpg)

**Applications** ->User can set application for created form.

    E.g. gst

**Product** ->User can set product for created form.

    E.g->GstNirvana,ASP

**Key** ->User can set form key in this block,it is should be unique for publisher and product.

    E.g. frmgstSaleInvoice

**Type** ->User can set type of form in this block.

    E.g. Form

**Name** ->User can set form name for display in this block.

**Sort index** ->User can set sontindex for created form it is require for sequencing for right click options.

**ClassPath** ->User can set classpath for created form in which form is defined.

    Eg.risersoft.app.gst

>Names Tab

![](/images/namestab.jpg)

**Add Text** ->User can set caption Name for right click option with prefix Add

    Eg.Add Sale Invoice

**Edit Text** ->User can set Edit Key word which showing before right click option when form is edit.

**Copy Text** ->User can set Caption for right click option when need to copy form.

>Applications Tab

![](/images/applicationstab.png)

**Adminbehave** -> Need to set value of Adminbehave for accessibility as per below:

*S=Require Super Admin*

*T=Require Tenant Admin*

*I=Ignore*

*A=Allow*


**Object Permission Role** -> No need to make any changes for those objects which are called directly in MainMenuXML and If objects are not called directly in MainMenuXML then find all possible navigation for called these objects & set  the parent object's keys with , if found more than one. We can enter cross object type parent by specifying *viewdef.key or frp.key or bro.key*

    eg: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice


**Platforms** ->User can set platform for created form like window,web etc

**In Context Menu** ->User can marked if required right click menu for edit.

**Report App Code** -> The prefix of the reportdataprovider should either be first appcode of entry in clientfrmprn/clientparent or mentioned in reportappcode.

>Conditions Tab

**AddXML** ->User can set condition for right click menu for add form.

![](/images/AddXML.jpg)

**EditsysXML**->User can set condition for showing edit right click option.

![](/images/EditsysXML.jpg)

**Grid Condition** ->User can set condition for visible right click option on views

![](/images/formreportfunctiongridcondition.jpg)

>Children Tab

![](/images/formreportfunctionchildrentab.png)

## List

Click on AppSystem -> Form/Report/Functions

![](/images/formreportfunctionlist.jpg)

## Edit

Click on AppSystem ->Form/Report/Functions ->Right Click ->Edit Form/Report/Func

![](/images/editformreportfunction.jpg)
