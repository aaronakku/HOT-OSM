# Humanitarian OpenStreetMap

This project is my first contribution to FOSS.It contains selected social facility present within India that have been extracted and displayed with the help of Mapbox GL.

## Getting Started

The html code [index.html](https://github.com/aaronakku/HOT-OSM/blob/master/index.html) contains the set of OSM data that has been extracted from map tiles of India. 
Along with this project i have learned to build Tile Server using the mbtiles of any place.

## Things i have done
1.  Extract Data based on OSM Tag.
2.  Used the extracted data and mapped with help of Mapbox GL.
3.  Visualized Map by making Tile Server(Click [Here](https://medium.com/@snehamariamsanthosh/making-of-tile-server-2ba9d397acc)
## Prerequisites
**In order to Extract data for map , the following set of commands are followed and also for mbtiles of various countries:**

` https://osmlab.github.io/osm-qa-tiles/country.html`

(Commands to be pasted onto Terminal)

```
sudo apt-get update

sudo apt-get install git-core

git — version

git clone https://github.com/mapbox/osm-tag-stats.git

cd osm-tag-stats

<sudo> npm install

<sudo> npm link
```
Save the filter JSON file in the same folder as the corresponding country’s mbtiles file.
* Name of the filter JSON file: filter.json[(here)](https://github.com/aaronakku/HOT-OSM/blob/master/filter.json)
* Command:
` osm-tag-stats — geojson=results.geojson — mbtiles=”india.mbtiles” — filter=’filter.json’ — count `

Once you’re done with the second command, copy paste the contents of results.geojson on https://geojson.io.

**Visualizing map using the help of Mapbox GL using the data extracted:**


Visualized final map
