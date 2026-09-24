# How to Wrap the Title of a Syncfusion Blazor Chart

## Overview

This sample demonstrates how to wrap long chart titles in a Syncfusion [Blazor Charts](https://www.syncfusion.com/blazor-components/blazor-charts) component when the title text exceeds the available width. The implementation configures the chart title to automatically flow onto multiple lines instead of being truncated or overflowing beyond the chart area. This approach improves readability when displaying descriptive chart titles in dashboards, reports, and analytics applications.

The sample uses the chart title styling API to control text overflow behavior and shows how the title is rendered when the available chart width is limited.

## Key Features

- Renders a chart using the `SfChart` component.
- Sets a long title using the `Title` property to demonstrate overflow behavior.
- Uses the `ChartTitleStyle` configuration element to customize title rendering.
- Sets `TextOverflow="TextOverflow.Wrap"` to automatically wrap lengthy title text onto multiple lines.
- Configures the primary X-axis using `ChartPrimaryXAxis`.
- Sets `ValueType="ValueType.Category"` for category-based axis values.
- Displays data using a `ChartSeries` component.
- Uses `Type="ChartSeriesType.Column"` to render a column chart.
- Binds chart data through the `DataSource` property.
- Maps category and value fields using the `XName` and `YName` properties.
- Demonstrates data binding with a `ChartData` model containing `X` and `Y` properties.

## Prerequisites

1. [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
2. [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open the project file:

   `TitleWrap.csproj`

3. Restore NuGet packages.
4. Build the project.
5. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Clone or download this repository.
2. Open the repository folder in Visual Studio Code.
3. Open the integrated terminal.
4. Navigate to the project directory:

```bash
cd TitleWrap
```

5. Restore NuGet packages:

```bash
dotnet restore
```

6. Run the application:

```bash
dotnet run
```

7. Open the local URL displayed in the console output.

## Project Structure

`Pages/Index.razor` - Demonstrates the `SfChart` implementation, chart title configuration, and title wrapping behavior.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- For documentation related to chart titles and title customization, see the Syncfusion Blazor Chart documentation: https://help.syncfusion.com/chart-sdk/blazor/charts/getting-started-with-web-app

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.