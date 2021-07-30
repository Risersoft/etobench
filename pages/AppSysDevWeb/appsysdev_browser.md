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

![](/images/browserdefinitiontabweb.png)

**<ROOT> & </ROOT>**: Root tag is body syntax.
    
**How to define BrowserID**:

< ID>BROWSEID< /ID>: This tag used to define browser id.

   E.g : <ID>BROWSEID</ID>

**How to set display grid**:

< DISPGRID>< /DISPGRID>: This tag used to set display grid.
   
   E.g:
   
  < DISPGRID>
  < VIEW KEY="viewCustomer" />
  < /DISPGRID>
  
**How to define a tree**:

< TREE>< /TREE>: Tree tag is body syntax.

**How set Sql for data source**:

< _DT>: Using this we can set sql for data source.

  E.g:
  
< _DT KEY="o" SQL="select CustomerID,isnull(Title,'')+' '+isnull(FirstName,'')+' '+isnull(MiddleName,'')+' '+isnull(LastName,'') as Customer from  Sales.Customer INNER JOIN Person.Person  ON Customer.PersonID = Person.BusinessEntityID where CustomerID = $BROWSEID$ order by Title,FirstName" />

**How to define local variable to store values**:

< _SET>: This tag used to define variable for store data locally.

  E.g:
  
< _SET VAR="CUST" VALUE="#MEMBER($o$,CustomerID)#" />

**How to add a Node**:

< NODE>: Using this tag we can define Node as per requirement.

  E.g:
  
< NODE PARENT="ID1"  KEY="Custso" CAPTION="Sale Orders">

*NODE PARENT*: Using this we can set parent id for to be added node.
*KEY*:Using this we can set key for to be added node.
*CAPTION*:Using this tag we can set caption for added node.

**How to set view for added node**:

< VIEW KEY >: using this tag we can set view for added node.

< VIEW KEY="ListAdvdemCustomer">

*FILTER KEY*
              
< FILTER KEY="customer">
< VALUE VALUE1="$CUST$" />
< /FILTER>
< /VIEW>


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
