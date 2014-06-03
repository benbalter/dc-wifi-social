# The Last Mile


### Bike and walk friendly routes to get to RDI Anchorage's new office.

Last summer RDI Anchorage moved into a new office space that was much-improved in many ways.  One thing that wasn't improved however, was access via human-powered means.  We've moved closer to the heart of midtown and away from the Campbell Creek Trail, which used to take us right to RDI's back door.  Aas luck would have it, that trail was greatly improved at the exact time we moved out!

Now, as the weather has turned warmer, many RDIers have been wondering about the best way to get to the new office by bike or foot (or skate board, or ski, or whatever).  This repository is an attempt to improve the last mile of your non-motorized commute by sharing route information.

It is also an excuse to play with GitHub's GeoJSON capabilities.

### [View The Map](routes.geojson)

## How to contribute

1. Clone the repo
2. Add your route to the routes.geojson file, in GeoJSON format
3. Submit a pull request


## How to get your route into GeoJSON format

If you use a GPS device, chances are you can download the route from your app's website in .gpx format.  Then you can use a [GPX to GeoJSON converter](http://mapbox.github.io/togeojson/) to convert it.  After you convert it, you'll probably want to delete the first half of the points, so everyone doesn't see exactly where you live.  Only the last mile or so is important. 

## Validating the geoJSON

When you submit a pull request, it will automatically check to ensure your geoJSON is valid.

If you'd like to check yourself, you can run `./script/cibuild` locally, or pasting the contents of `bars.geojson` into http://geojsonlint.com.
