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
 
![](/images/definition-form-example.jpg)

![](/images/definition-form-tag.png)


**Step-2** ->We can define combos using below xml codes.

![](/images/definition-define-combo.png)

**2.1.** *Combos* -> We can use tags for combos < combos > as starting tag < /combos > as ending tag.

**2.2** *Table* -> We can use tags for table <table> as starting tag </table> as ending tag and set lookup sql for combos between <table> and </table>.

**2.3** *Key* -> We set key name for lookup sql between tags < key > and < /key >.
   
![](/images/definition-key-example.jpg)

**2.4** *Sql* -> We can put sql query between tags < sql > and < /sql >

![](/images/definition-sql-example.jpg)

**Step-3** : We can map combo’s key with lookup key in this section : 

**3.1** *Lookups* -> -> We can map combo’s key with mainSql’s columns and childrensql’s columns under formatxml (between < formatxml > and < /formatxml >) or prepeditxml (between < prepeditxml > and < /prepeditxml >) section like this.

![](/images/definition-map-combokey.png)

**3.2** *Key Field* -> we can use tags for define key field using key word < KEY > as starting tag < /KEY > as ending tag. 

**3.3** *Caption* -> we can set caption for key field as per require using key word CAPTION.

  E.g-> CAPTION="Customer"

**3.4** *Lookupkey* -> we can set lookupkey as per define in columns between < KEY > and < /KEY > it should be unique and correct. 

  Define Lookupkey:
  
![](/images/definition-Lookupkey-order.png)

  UseLookupKey:  

![](/images/definition-UseLookupKey-order.png)


**Step-4** -> We can define vlists using below tags like this.

![](/images/definition-define-vlist.png)


**4.1** We can map vlist’s key with mainSql’s columns and childrensql’s columns under formatxml (between < formatxml > and < /formatxml >) or prepeditxml (between < prepeditxml > and < /prepeditxml >) section like this. 

![](/images/definition-map-vlistkey.png)

**Step-5** -> We can define mainsql like this. 

![](/images/definition-define-mainsql.png)

**5.1** *mainsql* -> We can use tags for define mainsql < mainsql > as starting tag < /mainsql > as ending tag and put required sql query for my row between < mainsql > & < mainsql >.

![](/images/definition-mainsql-example.jpg)


**5.2** *IDField* ->we can put idfied between tags < IDField > and < /IDField >.

![](/images/definition-idfield-example.jpg)

**5.3** *ReqFields* ->using this tag we can mention mandatory columns.

![](/images/definition-reqfields-example.jpg)

**5.4** *DescripTemplate* -> using this tag we can columns for description.

![](/images/definition-descriptemplate-example.jpg)

**5.5** *formatxml* -> using this tag we formatting of visible columns and set caption for columns as per requirement.

![](/images/definition-formatxml-example.jpg)

	 
**Step-6** -> We can define childrensql like this.

![](/images/definition-define-childrensql.png)

**6.1** *Children* -> we can use tags for define children < children > as starting tag ,</children > as ending tag.

**6.2** *Child*->under this tag we can define Children items properties < child> is starting tag </child > is ending tag.

**6.3** *Key* ->Using this tag we set key for children’s sql and < key> is starting tag </key> is ending tag. 

![](/images/definition-key2-example.jpg)

**6.4** *Sql* -> we can use this tags for set sql query and used < sql > as starting tag < /sql > as ending tag and put required sql query between < sql > & < sql >.

![](/images/definition-sql2-example.jpg)

**6.5** *ReqFields* ->We can used this tag for mention mandatory columns same as main sql.

**6.6** *reversedirection* ->using this tag we can set visibility of columns from left to right OR right to left.

![](/images/definition-reversedirection-example.jpg)


**6.7** *formatxml* -> using this tag we formatting of visible columns and set caption for columns as per requirement same as main sql.

**6.8** *prepeditxml* ->using this tag we can set idfield for children’s sql query.

![](/images/definition-prepeditxml-example.jpg)
   
![](/images/weboutput-salesorder-heading.png)

![](/images/definition-weboutput-salesorder.png)

