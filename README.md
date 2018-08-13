# og-prod-reporting-trends

## Overview

og-prod-reporting-trends is a Predix UI component

## Description

Component used to create four column chart layout with production trend charts.

1. Each page holds four production charts.
2. If there is no chart data in a page, it will be shown as a place holder with grey boxes.
3. Each page can be navigated using the pagination.
4. Handles chart column resizing based on the parent container size.

## Usage

<og-prod-reporting-trends data='{{data}}'></og-prod-reporting-trends>

## Properties

data: json array | null | undefined = {}notify
This property provides the data for the charts and layout.

heightDifference: Number | null | undefined = 60notify
This property provides the difference of height used to calculate each chart column's height based on the wrapper height property, Math.min(this.minHeight = 300,(this.wrapperHeight - this.heightDifference) / 2).

showLegends: Boolean = falsenotify
Including this property will show the legend panel.

```
<og-prod-reporting-trends show-legends></og-prod-reporting-trends>
```

showSubTitle: Boolean = falsenotify
Including this property will show the sub title.

```
<og-prod-reporting-trends show-sub-title></og-prod-reporting-trends>
```

showTrendIcon: Boolean = falsenotify
Including this property will show the trend arrow icons.

```
<og-prod-reporting-trends show-trend-icon></og-prod-reporting-trends>
```

showTrendSubTitle: Boolean = falsenotify
Including this property will show the trend sub title.

```
<og-prod-reporting-trends show-trend-sub-title></og-prod-reporting-trends>
```

wrapperHeight: Number | null | undefined = 600notify
This property provides the height of the layout. Use both wrapperHeight and heightDifference property to define the card layout (padding/margin) to fit according to the SVG layout.

### Prerequisites

1. node.js
2. npm
3. bower
4. [webcomponents-lite.js polyfill](https://github.com/webcomponents/webcomponentsjs)

Node, npm and bower are necessary to install the component and dependencies. webcomponents.js adds support for web components and custom elements to your application.

## Getting Started

First, install the component via bower on the command line.

```
bower install og-prod-reporting-trends --save
```

Second, import the component to your application with the following tag in your head.

```
<link rel="import" href="/bower_components/og-prod-reporting-trends/og-prod-reporting-trends.html"/>
```

Finally, use the component in your application:

```
Insert Your demo code here.

<og-prod-reporting-trends
data='{"crude":{"name":"Oil","title":"Oil","unit":"Tonnes","subtitle":"(total for past 5 months)","trend_subtitle":"(vs previous month)","chart":{"data":{"x":["2018-03-10","2018-04-10","2018-05-10","2018-06-10","2018-07-10"],"y":[9521422,9631674,8972642.88,9053527,9881545],"use_actual_dates":true,"displayMode":"months","istimestamp":false},"layout":{"xaxis":{"tickformat":"%b"}},"trace":{"line":{"color":"#088230","dash":"solid","width":3}}}},"gas":{"name":"Gas","title":"Gas","unit":"MMSCF","subtitle":"(total for past 5 months)","trend_subtitle":"(vs previous month)","chart":{"data":{"x":["2018-03-10","2018-04-10","2018-05-10","2018-06-10","2018-07-10"],"y":[37659,37255,35076,37020,36187],"use_actual_dates":true,"displayMode":"months","istimestamp":false},"layout":{"xaxis":{"tickformat":"%b"}},"trace":{"line":{"color":"#F15854","dash":"dot","width":3}}}},"water_produced":{"name":"Water Produced","title":"Water Produced","unit":"BBL/D","subtitle":"(total for past 5 months)","trend_subtitle":"(vs previous month)","chart":{"data":{"x":["2018-03-10","2018-04-10","2018-05-10","2018-06-10","2018-07-10"],"y":[5050282,4623204,4533053,4215330,4581592],"use_actual_dates":true,"displayMode":"months","istimestamp":false},"layout":{"xaxis":{"tickformat":"%b"}},"trace":{"line":{"color":"#5ABEF6","dash":"dashdot","width":3}}}},"water_injected":{"name":"Water Injected","title":"Water Injected","unit":"BBL/D","subtitle":"(total for past 5 months)","trend_subtitle":"(vs previous month)","chart":{"data":{"x":["2018-03-10","2018-04-10","2018-05-10","2018-06-10","2018-07-10"],"y":[10645602,10364521,10630827,9809743,10463277],"use_actual_dates":true,"displayMode":"months","istimestamp":false},"layout":{"xaxis":{"tickformat":"%b"}},"trace":{"line":{"color":"#5ABEF6","dash":"solid","width":3}}}},"oil":{"name":"Oil","title":"Oil","unit":"Tonnes","subtitle":"(total for past 5 months)","trend_subtitle":"(vs previous month)","chart":{"data":{"x":["2018-03-10","2018-04-10","2018-05-10","2018-06-10","2018-07-10"],"y":[9521422,9631674,8972642.88,9053527,9881545],"use_actual_dates":true,"displayMode":"months","istimestamp":false},"layout":{"xaxis":{"tickformat":"%b"}}}}}'>
</og-prod-reporting-trends>
```

<br />
<hr />

## Documentation

Read the full API and view the demo [here](https://predixdev.github.io/og-prod-reporting-trends).

The documentation in this repository is supplemental to the official Predix documentation, which is continuously updated and maintained by the Predix documentation team. Go to [http://predix.io](http://predix.io) to see the official Predix documentation.

## Local Development

From the component's directory...

```
$ npm install
$ bower install
$ gulp sass
```

From the component's directory, to start a local server run:

```
$ gulp serve
```

Navigate to the root of that server (e.g. http://localhost:8080/) in a browser to open the API documentation page, with link to the "Demo" / working examples.

### GE Coding Style Guide

[GE JS Developer's Guide](https://github.com/GeneralElectric/javascript)

<br />
<hr />

## Known Issues

Please use [Github Issues](https://github.com/PredixDev/og-prod-reporting-trends/issues) to submit any bugs you might find.
