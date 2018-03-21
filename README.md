# Humanitarian OpenStreetMap

This project is my first contribution to FOSS.It contains selected social facility present within India that have been extracted and displayed with the help of Mapbox GL.

## Getting Started

The html code [index.html](https://github.com/aaronakku/HOT-OSM/blob/master/index.html) contains the set of OSM data that has been extracted from map tiles of India. 
Along with this project I have learned to build Tile Server using the mbtiles of any place.

## Things i have done

1.  Extract data based on OSM tag.
2.  Used the extracted data and mapped with help of Mapbox GL.
3.  Visualized map by making Tile Server(Click [Here](https://medium.com/@snehamariamsanthosh/making-of-tile-server-2ba9d397acc))

## Prerequisites

**In order to Extract data for map , the following set of commands are followed and for downloading mbtiles of various countries:**

(paste following link)
  
` https://osmlab.github.io/osm-qa-tiles/country.html`

The link used within index.html point to india.mbtiles file
you can say download india.mbtiles file from

Link: https://osmlab.github.io/osm-qa-tiles/country.htm
 
(Commands to be pasted onto Terminal)

`wget <link to india.mbtiles>`

```
sudo apt-get update

sudo apt-get install git-core

git --version

git clone https://github.com/mapbox/osm-tag-stats.git

cd osm-tag-stats

<sudo> npm install

<sudo> npm link
```
Save the filter JSON file in the same folder as the corresponding country’s mbtiles file.
* Name of the filter JSON file: filter.json[(here)](https://github.com/aaronakku/HOT-OSM/blob/master/filter.json)
* Command:

  ` osm-tag-stats --geojson=results.geojson --mbtiles="india.mbtiles" --filter='filter.json' --count `

Once you’re done with the second command, copy paste the contents of results.geojson on https://geojson.io.

An Overview of extracted data([here](https://github.com/aaronakku/HOT-OSM/blob/master/results.geojson))

**Visualizing map with the help of Mapbox GL using the data extracted:**

Visualized final map[(here)](https://github.com/aaronakku/aaronakku/blob/master/README.md)

## The Making Of Reusable Map
Once the data extracted , clubbing the result of extracted data on to an html page[(index.html)](https://github.com/aaronakku/HOT-OSM/blob/master/index.html) is to be done.
With help of Mapbox ,using the following example[(here)](https://www.mapbox.com/mapbox-gl-js/example/simple-map/).
and for additional reference the following links were refereed :
```
https://www.mapbox.com/mapbox-gl-js/style-spec/#layers

https://www.mapbox.com/mapbox-gl-js/api/
```
It contains the basic code to display a map and combining the extracted data results in creating the [reusable map](https://aaronakku.github.io/aaronakku/INTERACTIVE-MAP/).
