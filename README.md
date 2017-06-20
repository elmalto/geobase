## Overview


Version: 1.0.0

API Scaladoc: [GeoBase](http://todo)

Scala wrapper around opentraveldata (geo/travel data).

Provides geographical mappings at airport/city/country level mainly based on
[opentraveldata](https://github.com/opentraveldata/opentraveldata) as well as
other mappings such as airlines or currencies. This facility also provides
classic time-oriented methods such as trip duration computation.

Geo/Travel facilities:

* Airport to City converter
* Airport/City to Country converter
* Airport/City/Country to Continent converter
* Airport/City/Country to IATA zone converter
* City/Country to Currency code converter
* Airline to Country converter
* Distance getter between two airports/cities
* Trip Type getter (domestic, continental or intercontinental)
* Conversion from local time to GMT time (without needing to know the GMT offset) (and vice et versa)
* A Segment EFT getter for local dates (without needing to know the GMT offset)
* A way to retrieve nearby airports within a defined radius


## Using geobase:


The full list of methods is available at [GeoBase doc](http://todo)

	import com.geobase.GeoBase

	val geoBase = new GeoBase()

	assert(geoBase.getCityForAirport("CDG") == "PAR")


## Including geobase to your dependencies:


With sbt, just add this line to your build.sbt:

	libraryDependencies += "geobase" % "geobase" % "1.0.0" from "http://todo/geobase/1.0.0/geobase-1.0.0.jar"