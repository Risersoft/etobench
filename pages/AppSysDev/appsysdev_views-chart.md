---
title: Chart
keywords: Chart
sidebar: appsysdev_sidebar
permalink: appsystem-developer/views-chart.html
folder: AppSysDev
hide_sidebar: false
comments: false
---

# Chart Tab

## ChartXML

![](/images/chartxml.jpg)

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

![](/images/chartxmloutput.png)

## Types of Chart 

Currently we have used ChartType=Column, LineSymbols, Pie,Area.. etc. in appsystem

**Column**: we can use column chart type like this: < ChartType> Column < /ChartType>

![](/images/columnchart.png)

**LineSymbols**: we can use column chart type like this: < ChartType> LineSymbols < /ChartType>

![](/images/linechart.png)

**Pie**: we can use column chart type like this: < ChartType>pie< /ChartType>

![](/images/piechart.png)

**Area**: we can use column chart type like this: < ChartType>Area< /ChartType>

![](/images/areachart.png)

We can also see different charts effect clicking on select button and select chart type.

![](/images/chartselection.png)


