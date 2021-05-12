---
title: Entities
keywords: Entities
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/entities.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---


# Entities

## Create

Click on AppSystem ->New->New Entity

![](/images/entityweb.png)

>Entity Tab

User create new entity here.

**Entity**->Set Entity name in this Field.

    E.g- D

**Description Entity**->User can set description of entity here.

    E.g-Department

**SysTable**->User can select systableid from combo

    E.g- SalesorderId

**Product**->User can select Product for entity

**Select View Key**->User can set View for default output for created output.

    E.g-listresourcegrp

**Select View Filter**->User can set Filter key for showing view output with filter key.

>Grid Condition Tab

User can set conditions which should be available on view’s Grid. Conditions should de define in XML format and syntax should be correct.

    E.g-  < COL KEY="ISCREW">< VALUE VALUE1="false"/>< /COL>
	
    ISCREW-column name and false it’s value

![](/images/gridconditiontabweb.png)

>Children Tab

User can add accessibility of Systableid for other Products.

![](/images/entitychildrentabweb.png)

**1. Product**->User can set Products for accessibility of systableid.

     E.g. Adventure Demo

**2. AppList**->User can set applist here.

     E.g. adm

## List

Click on AppSystem -> Entities

![](/images/entitylistweb.png)

## Edit

Click on AppSystem -> Entities->Right Click->Edit Entity

![](/images/editentityweb.png)
