---
title: Applications
keywords: Applications
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/applications.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---

# Applications

## Create

There are two options to create applications:

1.	New -> New Application

2.	AppSystem -> Applications->Right Click ->Copy App..

After choosing any one option, the application form will appear.

![](/images/applicationweb.png)

>Application Options Tab


**ApplicationID** ->Need to set integer value it is Compulsory and Unique for particular publisher.

     E.g. ApplicationID=1

**ApplicationCode**  ->User can set code for new application like kasp.
     It should be unique for Publisher and Product.

    E.g. ApplicationCode= kasp

**ApplicationCode2** ->User can set ApplicationCode2 if user want to assign all functionality of existing application.

    E.g. ApplicationCode= gst

**ApplicationName** ->User can set application Name for display.

    E.g. ApplicationCode= ASP Solution
	
**Product** ->User can select a Product for application it is compulsory.

    E.g.ASP	

**Data DB Name** ->User can set Default Database Name here.

    E.g. Data DB Name = mxgstdb
	
	
**Not Listed** ->Default value for this in False if user not wants to show application in Appstarter Select Menu then marked it.
	

**Adminbehave** -> Need to set value of Adminbehave for accessibility as per below:

*S=Require Super Admin*

*T=Require Tenant Admin*

*I=Ignore*

*A=Allow*


**Object Permission Role** -> No need to make any changes for those objects which are called directly in MainMenuXML and If objects are not called directly in MainMenuXML then find all possible navigation for called these objects & set  the parent object's keys with , if found more than one. We can enter cross object type parent by specifying *viewdef.key or frp.key or bro.key*

    eg: viewkey.ListInvoice or frp.frmInvoice or bro.Invoice



>Menu Definition Tab

User can define application menu’s here in XML format.

!![](/images/menudefinitiontabweb.png)

##### **Body Syntax**->

**&lt;ROOT>**      

  **&lt;TOOLBAR** KEY="mnuMain" BEFORE="1">     

   **&lt;/TOOLBAR>**    

**&lt;/ROOT>**

##### **Define Menu Name**-> 

We can define menu name using below xml tags.

![](/images/DefineMenuNameXML.png)

_**Description**_:

**&lt;TOOL> &lt;/TOOL>**: Starting & Ending Tag

**STYLE**: we can use Style tag for menu category

    E.g-> STYLE="MNU"

**NAME**: We can use Name tag for define menu name as per requirement

    E.g-> NAME="Human Resources"

**KEY**: Every menu & menu items have a unique key, we set key like this.

    E.g-> KEY="ID_mnuadvdemHR"

**ICON**: we can give image name in this tag for menu like this.

    E.g-> ICON= "HumanResources.png"
	
**Output**->

!![](/images/DefineMenuNameOutput.png)


##### **Listing Option Syntax**->

We can define sub menus using below xml tags.

!![](/images/ListingMenuXML.png)

_**Description**_:

**&lt;TOOL> & &lt;/TOOL>**: Starting & Ending Tag

**STYLE**: we can use Style tag for menu category.

    E.g-> STYLE="BUT"

**NAME**: We can use Name tag for define menu name as per requirement

    E.g-> NAME="Department"

**KEY**: Every menu & menu items have a unique key, we set key like this.

    E.g-> KEY="ID_AdvDep"

**TAG**: We can set view key for submenu between <TAG> and </TAG> like this.

   &lt;TAG>           

   &lt;VIEW KEY="ListAdvdemDepartment"/>        

   &lt;/TAG>   

##### **New Menu**-> 

We can define ne menu using below xml tags.

!![](/images/NewMenuXML.png)


_**Description**_:

**BG** ->Used for separator between two menus.

   E.g-> BG="1"


**STYLE** -> Need to set BUT for SubMenu.

**NAME** ->User can set New menu  in this block.

    E.g-> New Application

**KEY**->User can set Keys for new menu in this block. It is should be Unique.

    E.g-> ID_NewApp

**CAT**-> User can set Category in this block.

    E.g->CAT

**TAG** ->All Forms and views key should be define between
&lt;TAG> and &lt;/TAG>

**FRM  KEY**->User Can set Form Key Name.

    E.g-> frmApp
	

![](/images/applicationfrmkey.png)

>Conditions Tab

**Data XML**

![](/images/dataxmlweb.png)

*OutPut* -> This Data XML is defined for grouping of List.

**Mobile Menu XML**

![](/images/mobilemenuxmlweb.png)

*Tags For Body Syntax:*

< ROOT>

< TOOLBAR KEY="mnuMain" BEFORE="1">

< /TOOLBAR>

< /ROOT>


*Tags for Menu:*

< TOOL BG="1" KEY="ID_Myprofile" STYLE="BUT" NAME="My Profile" ICON = "MyProfile.png">

< TAG>

< VIEW KEY="ViewMyProfile"></VIEW>

< /TAG>

< /TOOL>

*Tags for Image Icon:*

We can used ICON for item menu image.
  
     Eg. ICON = "MyProfile.png"
   
*OutPut:*

![](/images/mobileiconweb.png)



>Info Tab

![](/images/infotabweb.png)

**StartUp Tool**->Set Menu keys for default output when application run.

This is defined in MenuDefinition.

     E.g. ID_Bnt for List of Branches

**MainForm**-> frmMain

**ObjPermission**->Set Objects Table/Function which is should be available in set Database.

    E.g Invoice

**ClassPath**->set class path in which application define

    E.g. kpmg.app.asp

**FontSize**->Set Default font size of text.

     E.g ->8.25

**AllowDefault**->Marked

**CommonMenu**->Marked for Showing Default common Menu’s.

![](/images/commonmenuweb.png)


## List

Click on AppSystem -> Applications

![](/images/applicationslistweb.png)

## Edit

Click on AppSystem -> Applications->Right Click->Edit In App Editor

![](/images/editapplicationweb.png)
