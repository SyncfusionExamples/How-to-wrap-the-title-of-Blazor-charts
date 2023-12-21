# How-to-wrap-the-title-of-Blazor-charts

This article explains how to wrap the chart title in Blazor Chart Component.

**Chart title wrap using TextOverFlow property**

The title of the [Blazor Chart](https://www.syncfusion.com/blazor-components/blazor-charts) is crucial for better comprehension of its usage. In the case of having a multi-line title, you can wrap it by setting the [TextOverFlow](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.TextOverflow.html) property in [ChartTitleStyle](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.ChartTitleStyle.html#Syncfusion_Blazor_Charts_ChartTitleStyle__ctor) to [Wrap](https://help.syncfusion.com/cr/blazor/Syncfusion.Blazor.Charts.TextOverflow.html#Syncfusion_Blazor_Charts_TextOverflow_Wrap). 

The following code example illustrates this.

**Index.razor**

```cshtml

@using Syncfusion.Blazor.Charts

<SfChart Width="500px" Title="This Example shows how to wrap the chart title to next line in case of overflow">

    <ChartPrimaryXAxis ValueType="Syncfusion.Blazor.Charts.ValueType.Category" />

    <ChartTitleStyle TextOverflow="TextOverflow.Wrap"></ChartTitleStyle>

    <ChartSeriesCollection>
        <ChartSeries DataSource="@MedalDetails" XName="X" YName="Y" Type="ChartSeriesType.Column" >
        </ChartSeries>
    </ChartSeriesCollection>

</SfChart>

@code {

    public class ChartData
    {
        public string X { get; set; }
        public double Y { get; set; }
    }

    public List<ChartData> MedalDetails = new List<ChartData>
    {
        new ChartData { X= "South Korea", Y= 39.4 },
        new ChartData { X= "India", Y= 61.3 },
        new ChartData { X= "Pakistan", Y= 20.4 },
        new ChartData { X= "Germany", Y= 65.1 },
        new ChartData { X= "Australia", Y= 15.8 },
        new ChartData { X= "Italy", Y= 29.2 },         
    };
}

```

The following screenshot illustrates the output of the above code snippet.

**Output:**

![](/Title-Wrap.png)

**Conclusion**

I hope you enjoyed learning how to wrap the title in Blazor Chart Component.

You can refer to our [Blazor Chart feature tour](https://www.syncfusion.com/blazor-components/blazor-charts) page to know about its other groundbreaking feature representations and [documentation](https://blazor.syncfusion.com/documentation/chart/getting-started), and how to quickly get started for configuration specifications. You can also explore our [Blazor Chart example](https://blazor.syncfusion.com/demos/chart/line?theme=bootstrap5) to understand how to create and manipulate data.

For current customers, you can check out our components from the [License and Downloads](https://www.syncfusion.com/sales/teamlicense) page. If you are new to Syncfusion, you can try our 30-day [free trial](https://www.syncfusion.com/downloads/blazor) to check out our other controls.

If you have any queries or require clarifications, please let us know in the comments section below. You can also contact us through our [support forums](https://www.syncfusion.com/forums), [support portal](https://support.syncfusion.com/create), or [feedback portal](https://www.syncfusion.com/feedback/blazor-components?control=charts). We are always happy to assist you!