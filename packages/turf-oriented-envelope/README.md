# @turf/oriented-envelope

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

## orientedEnvelope

Takes any number of features and returns a rotated rectangular [Polygon][1] that encompasses all vertices.

Based on the [geojson-minimum-bounding-rectangle][2]
package by Matthias Feist.

### Parameters

*   `geoJsonInput` **AllGeoJSON**&#x20;
*   `options` **{minimizeWidth: [boolean][3]?}**  (optional, default `{}`)
*   `geojson` **[GeoJSON][4]** input features

### Examples

```javascript
var features = turf.featureCollection([
  turf.point([-75.343, 39.984], {"name": "Location A"}),
  turf.point([-75.833, 39.284], {"name": "Location B"}),
  turf.point([-75.534, 39.123], {"name": "Location C"})
]);

var enveloped = turf.orientedEnvelope(features);

//addToMap
var addToMap = [features, enveloped];
```

Returns **[Feature][5]<[Polygon][1]>** a rotated rectangular Polygon feature that encompasses all vertices

[1]: https://tools.ietf.org/html/rfc7946#section-3.1.6

[2]: https://www.npmjs.com/package/geojson-minimum-bounding-rectangle

[3]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean

[4]: https://tools.ietf.org/html/rfc7946#section-3

[5]: https://tools.ietf.org/html/rfc7946#section-3.2

<!-- This file is automatically generated. Please don't edit it directly. If you find an error, edit the source file of the module in question (likely index.js or index.ts), and re-run "yarn docs" from the root of the turf project. -->

---

This module is part of the [Turfjs project](https://turfjs.org/), an open source module collection dedicated to geographic algorithms. It is maintained in the [Turfjs/turf](https://github.com/Turfjs/turf) repository, where you can create PRs and issues.

### Installation

Install this single module individually:

```sh
$ npm install @turf/oriented-envelope
```

Or install the all-encompassing @turf/turf module that includes all modules as functions:

```sh
$ npm install @turf/turf
```
