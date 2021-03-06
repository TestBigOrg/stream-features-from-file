# stream-features-from-file

[![Build Status](https://travis-ci.org/mapbox/stream-features-from-file.svg?branch=master)](https://travis-ci.org/mapbox/stream-features-from-file)

Streams GeoJSON features from a file.

Supports the following source formats:
- GeoJSON (`FeatureCollection` only!)
- CSV
- Shapefile

Non-GeoJSON formats are read by [Mapnik](http://mapnik.org/documentation/node-mapnik/3.5/).

## Usage

```js
const featureStream = streamFeaturesFromFile(filePath);
```

`streamFeaturesFromFile` accepts a `filePath` argument and returns a readable object-mode stream of GeoJSON features derived from the provided file.
