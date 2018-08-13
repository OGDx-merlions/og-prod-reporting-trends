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
Including this property like <og-prod-reporting-trends show-legends></og-prod-reporting-trends> will show the legend panel.

showSubTitle: Boolean = falsenotify
Including this property like <og-prod-reporting-trends show-sub-title></og-prod-reporting-trends> will show the sub title.

showTrendIcon: Boolean = falsenotify
Including this property like <og-prod-reporting-trends show-trend-icon></og-prod-reporting-trends> will show the trend arrow icons.

showTrendSubTitle: Boolean = falsenotify
Including this property like <og-prod-reporting-trends show-trend-sub-title></og-prod-reporting-trends> will show the trend sub title.

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
