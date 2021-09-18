---
title: Data Source
keywords: Data Source
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/views-datasource.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---


# DataSource Tab

User can set data source SQL for view output in this section.

![](/images/viewdatasourcetabweb.png)

**AppliFilters** ->User can set list of filters which are applicable on this view.

    E.g- Comp,Campus ..etc
	
![](/images/viewapplifiltersweb.png)

**Type** ->User can set Data source query type Default value is Fields but user can it to Template as per requirement.

![](/images/viewtypeweb.png)

**View Width Percent** ->User can set view’s output percentage.

![](/images/viewwidthperweb.png)

**Ignore Paging** ->Default value for this is False but user can set True if paging require on view output.

![](/images/viewignorepagingweb.png)

## Fields Tab

![](/images/viewfieldstabweb.png)

**Select**-> User can set fields of Data source Query without select and Form keywords.

![](/images/viewselectweb.png)

**From**-> User can set Data Source Tables or Functions.

![](/images/viewfromweb.png)

**Client**-> User can use Client if DataSoursce is PDCClientView

![](/images/viewclientweb.png)

**Group By**-> User can set Group by Fields of select query.

![](/images/viewgroupbyweb.png)

**Having**-> If SQL query included Having Condition then user can set having condition in this section.

![](/images/viewhavingweb.png)

**Order BY**-> User can set Order columns in this section.

![](/images/vieworderbyweb.png)

**Fixed Where**-> User can set fixed where conditions in this section.

![](/images/viewfixedwhereweb.png)

**ObjPermission**-> User can set Object which must be present in that Product.

![](/images/viewobjpermissionweb.png)


## Parameters Tab

![](/images/parameterstabweb.png)

**FiltParam**-> User can set fixed filter with default value in this block.

**Note**: FiltParam should be in XML Code and use correct Syntax. If syntax not correct then errors showing in Errors block and applied Filters should be present in AppliFilters List.

    E.g.

![](/images/FiltParamweb.png)

**&lt;FILTER>** ->Starting Tag.

**FILTER KEY**->Set Filter key define in Table ClientFilter

**ACTION**->Set Default

**VALUE VALUE1**->Set IdField like FinyearID.Function Currfinid pick current finyearid.

**OPERTYPE**->Set operation type like eq for Equal.

**&lt;/FILTER>** ->Ending Tag.

**Output**->

![](/images/filteroutputweb.png)

**WhereParam** ->

*How to Create where param:*

User can create user define where conditions as per requirement between starting tag & ending tag and apply particular on menu’s in menu definition.

     E.g: <INVSL> Starting Tag & </INVSL> ending tag.DocType=’IS’ User define condtion


![](/images/WhereParamweb.png)

*How to use where param:*

    E.g. Use WhereParam conditions in MenuDefination

![](/images/WhereParaminmenudifinationweb.png)


