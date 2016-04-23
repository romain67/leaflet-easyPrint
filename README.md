## leaflet-easyPrint

A simple [leaflet.js](http://www.leafletjs.com) plugin which allows users to print the map to an A4 page (landscape or portrait). Check out the [demo](http://rowanwins.github.com/leaflet-easyPrint/).

### Usage
**Step 1.** Include the required js and css files in your document. 

```html
   	<link rel="stylesheet" href="dist/easyPrint.css"/>
   	<script src="dist/leaflet.easyPrint.js"></script>
```

**Step 2.** Add the following line of code to your map script

``` js
L.easyPrint().addTo(map)
```

**Step 3.**
You can pass a number of options to the plugin to control various settings.

| Option        | Type         | Default      | Description   |
| ------------- |--------------|--------------|---------------|
| title | string | 'Print map' | Sets the text which appears as the tooltip of the print button |
| position | [Leaflet control position](http://leafletjs.com/reference.html#control-positions) | 'topleft' | Position the print button |
| A4Portrait | boolean | true | Displays a portrait button |
| A4Landscape | boolean | true | Displays a landscape button |

Here's an example of passing through some options.
``` js
L.easyPrint({
	title: 'My awesome print button',
	position: 'bottomright',
	A4Portrait: false
}).addTo(map);
```

### Acknowledgements
Huge hats off go to [mourner](https://github.com/mourner) and all the [contributors](https://github.com/Leaflet/Leaflet/graphs/contributors) to the leaflet.js project, it's an amazing piece of open source software!

And finally thanks to [IcoMoon](http://icomoon.io/) for the print icon.