---
title: Form Definition with Zero Code
keywords: Form Definition with Zero Code
sidebar: appsysdev_sidebar
permalink: appsystem-developer/form-definition-zero-code.html
folder: AppSysDev
hide_sidebar: false
comments: false
---


# Form Definition with Zero Code

>Definition Tab 

In this section, we have define definition of forms in XML format.

**Step-1** -> We can define definition of forms in XML format and used below tags.
 
  E.g.  <form>…. </form>


![](/images/definition-form-tag.png)


**Step-2** ->We can define combos using below xml codes.

![](/images/definition-define-combo.png)

**2.1.** *Combos* -> We can use tags for combos <combos> as starting tag </combos> as ending tag.

**2.2** *Table* -> We can use tags for table <table> as starting tag </table> as ending tag and set lookup sql for combos between <table> and </table>.

**2.3** *Key* -> We set key name for lookup sql between tags <key> and </key> 

  E.g. <key>Product</key>

**2.4** *Sql* -> We can put sql query between tags <sql> and </sql>

  E.g. 
  
  ```
    <sql>select Distinct.ProductID, Name from Sales.SpecialOffer Product</sql>

  ```
  

**Step-3** -> We can map combo’s key with mainSql’s columns and childrensql’s columns like this. (dt used for mainsql)

![](/images/definition-map-combokey.png)

**3.1** *Lookups* -> we can use tags for define lookups. <lookups> as starting tag </lookups> as ending tag.

**3.2** *field* -> we can put define combo’s key between <key> and </key> 

**3.3** *fieldname* -> we can set column’s name of mainsql or childrensql for mapping with defined combos.

  E.g . <fieldName>ProductID</fieldName>

**3.4** *tablename* -> we can put default table key dt for mainsql and defined table key for childrensql. 

  E.g-> dt for mainsql & Order for childrensql (see step.5&6)

![](/images/definition-tablename-order.png)


**Step-4** -> We can define vlists also using below tags.

![](/images/definition-define-vlist.png)


**4.1** We can map vlist’s key with mainSql’s columns and childrensql’s columns like this.

![](/images/definition-map-vlistkey.png)

**Step-5** -> We can define mainsql like this. 

![](/images/definition-define-mainsql.png)

**5.1** *mainsql* -> We can use tags for define mainsql <mainsql> as starting tag </mainsql> as ending tag and put required sql query for my row between <mainsql> & <mainsql>.

  E.g <mainSql>*select*from sales.SalesOrderHeader where Salesorderid = %frmidx%*</mainSql>

**5.2** *IDField* ->we can put idfied between tags <IDField> and </IDField>

  E.g. <IDField>Salesorderid </IDField>

**5.3** *ReqFields* ->using this tag we can mention mandatory columns.

  E.g <ReqFields>CustomerID, BillToAddressID, ShipToAddressID, OnlineOrderFlag </ReqFields>

**5.4** *DescripTemplate* -> using this tag we can columns for description.

  E.g-> <DescripTemplate>Order No. %Salesorderid% Dated %OrderDate% </DescripTemplate>

**5.5** *formatxml* -> using this tag we formatting of visible columns and set caption for columns as per requirement.

  E.g-> 
  
  ```
      <formatxml>
      <COL KEY="RevisionNumber" CAPTION="Revision No." />
      <COL KEY="OrderDate" CAPTION="Order Date"/>
      <COL KEY="SalesPersonID" CAPTION="Sales Person" />
      <COL KEY="TerritoryID" CAPTION="Territory" />
      <COL KEY="BillToAddressID" CAPTION="Bill To" />
      <COL KEY="rowguid" HIDDEN="true"/>
      <COL KEY="CreditCardID" HIDDEN="true"/>	
      <COL KEY="CurrencyRateID" HIDDEN="true"/>	
      </formatxml>
	  
  ```
	 
**Step-6** -> We can define childrensql like this.

![](/images/definition-define-childrensql.png)

**6.1** *Children* -> we can use tags for define children < children > as starting tag ,</ children > as ending tag.

**6.2** *Child*->under this tag we can define Children items properties < child> is starting tag </ child > is ending tag.

**6.3** *Key* ->Using this tag we set key for children’s sql and < key> is starting tag </ key> is ending tag. 

  E.g. -><key>Order</key>

**6.4** *Sql* -> we can use this tags for set sql query and used <sql> as starting tag </sql> as ending tag and put required sql query between <sql> & <sql>

  E.g 
  
  ```
    <sql> select * from sales.SalesOrderDetail where Salesorderid = %frmidx% </sql>

  ```
   

**6.5** *ReqFields* ->We can used this tag for mention mandatory columns same as main sql.

**6.6** *reversedirection* ->using this tag we can set visibility of columns from left to right OR right to left.

  E.g <reversedirection>false</reversedirection> 

**6.7** *formatxml* -> using this tag we formatting of visible columns and set caption for columns as per requirement same as main sql.

**6.8** *prepeditxml* ->using this tag we can set idfield for children’s sql query.

  E.g 
  
  ```
   <prepeditxml>
   <BAND INDEX="0" TABLE="sales.SalesOrderDetail" IDFIELD="SalesOrderDetailID"></BAND>
   
  ```
   
![](/images/weboutput-salesorder-heading.png)

![](/images/definition-weboutput-salesorder.png)

