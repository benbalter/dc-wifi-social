# [View The Map](https://render.githubusercontent.com/view/geojson?url=https://raw.githubusercontent.com/ResourceDataInc/last-mile/master/routes.geojson)

<img src="https://travis-ci.org/ResourceDataInc/last-mile.svg">

## The Last Mile

### Bike and walk friendly routes to get to RDI Anchorage's new office.

Last summer RDI Anchorage moved into a new office space that is much-improved in many ways.  One thing that isn't improved is access via human-powered means.  We've moved closer to the heart of midtown and away from the Campbell Creek Trail, which used to take us right to RDI's back door.  

Now, as the weather has turned warmer, many RDIers have been wondering about the best way to get to the new office by bike or foot (or skateboard, or ski, or whatever).  This repository is an attempt to improve the last mile of your non-motorized commute by sharing route information.  It is also an excuse to play with GitHub's GeoJSON capabilities.

Please contribute the last mile or so of your commute to this repository so that it may help fellow RDIers.

## How to contribute

1. Clone the repo
2. Add your route to the routes.geojson file, in GeoJSON format
3. Submit a pull request


## How to get your route into GeoJSON format

If you use a GPS device (smart phone, Garmin, etc.) and/or a fitness app (Strava, Endomondo, Garmin Connect, Map My Ride, etc.), you can download the route from your app's website in .gpx format.  Then use a [GPX to GeoJSON converter](http://mapbox.github.io/togeojson/) to convert it.  After you convert it, you'll probably want to delete the first half of the points, so everyone doesn't see exactly where you live.  Only the last mile or so is important. 

## Validating the GeoJSON

When you submit a pull request, it will automatically check to ensure your geoJSON is valid.

If you'd like to check yourself, you can run `./script/cibuild` locally, or pasting the contents of `routes.geojson` into http://geojsonlint.com.
