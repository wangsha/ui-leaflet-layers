# ui-leaflet-layers

Angular UI Leaflet Layers Plugin, it extend layer capabilities for [ui-leaflet](http://angular-ui.github.io/ui-leaflet)

### Supported Layers:

* Google Maps
* Bing
* Yandex
* China
* HeatLayer
* WebGLHeatMapLayer
* WFS
* UTFGrid
* [MapboxGL](https://github.com/mapbox/mapbox-gl-leaflet)

### Coming Soon:

* [Mapbox](http://mapbox.com/)
* [CartoDB](http://cartodb.com/)
* [esri-leaflet](http://esri.github.io/esri-leaflet/)

### MapboxGL Example

**Controller:**

```js
angular.extend($scope, {
  center: {
    lat: 38.91275,
    lng: -77.032194,
    zoom: 15
  },
  layers: {
    baselayers: {
      mapboxGlLayer: {
        name: 'Sample',
        type: 'mapboxGL',
        layerOptions: {
          accessToken: [token],
          style: 'mapbox://styles/mapbox/streets-v8'
        }
      }
    },
    overlays: {}
  }
})
```

**HTML:**

```html
<leaflet lf-center="center" layers="layers" height="480px" width="100%"></leaflet>
```
