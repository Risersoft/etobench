---
title: Chart
keywords: Chart
sidebar: appsysdevweb_sidebar
permalink: appsystem-developer-web/views-chart.html
folder: AppSysDevWeb
hide_sidebar: false
comments: false
---

# Chart Tab

## ChartXML

![](/images/chartxmlweb.jpg)

< clsChartModel >  is starting Tag & < /clsChartModel >  is ending tag of chart definition.

< Legend >  & < /Legend >  We can define orientation & position between starting & ending tag of Legend.

    E.g
	 
< Legend >        
< Orientation >Auto< /Orientation>   
< Position >None< /Position>    
< Title />    
< /Legend>

    
< ChartType> We can set chart type of charts like Column,LineSymbols,Pie,Area between <ChartType>  & </ChartType> 

< Series>   We can define multiple series for showing data grid between <Series> & </Series>.   
    
     Like this: 
	 
< Series>      
< clsSeriesModel> 
< ChartType>column</ChartType>      
< Binding>Empcount</Binding>          
< BindingX>GroupName</BindingX>     
< /clsSeriesModel>      
< /Series>   


< clsSeriesModel> We can define layout of chart’s series between < clsSeriesModel> & clsSeriesModel> 

< Binding> We can set column’s name which values we want to show horizontally or respect of Y axis.

< BindingX> We can set column’s name which values we want to show vertically or respect of X axis.
 
*Output ->*

![](/images/chartxmloutputweb.png)

## Types of Chart 

Currently we have used ChartType=Column, LineSymbols, Pie,Area.. etc. in appsystem

**Column**: we can use column chart type like this: < ChartType> Column < /ChartType>

![](/images/columnchartweb.png)

**LineSymbols**: we can use column chart type like this: < ChartType> LineSymbols < /ChartType>

![](/images/linechartweb.png)

**Pie**: we can use column chart type like this: < ChartType>pie< /ChartType>

![](/images/piechartweb.png)

**Area**: we can use column chart type like this: < ChartType>Area< /ChartType>

![](/images/areachartweb.png)

We can also see different charts effect clicking on select button and select chart type.

![](/images/chartselectionweb.png)


