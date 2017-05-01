Toronto Open Datasets
=====================

Most of Toronto's Open Data is financial or sociological, but here are some
that might be of interest to students in EEB. A lot of these are a bit
geospatial in nature. These are semi-ordered from least to most interesting.

* [Data catalogue](http://www1.toronto.ca/wps/portal/contentonly?vgnextoid=1a66e03bb8d1e310VgnVCM10000071d60f89RCRD)
* [Open Data license](http://www1.toronto.ca/wps/portal/contentonly?vgnextoid=4a37e03bb8d1e310VgnVCM10000071d60f89RCRD)

Licensed Dogs and Cats
----------------------

This is not totally serious, but it seemed interesting in a "fun" way. It's not
really raw data and most of the analysis is done anyway, so I don't think much
can be done with it by itself.

 * [Licensed Dog and Cat Names](http://www1.toronto.ca/wps/portal/contentonly?vgnextoid=8ba46ee592d79410VgnVCM10000071d60f89RCRD&vgnextchannel=1a66e03bb8d1e310VgnVCM10000071d60f89RCRD)
 * [Licensed Dogs and Cats Reports](http://www1.toronto.ca/wps/portal/contentonly?vgnextoid=0a7e1f46f71fb310VgnVCM10000071d60f89RCRD&vgnextchannel=1a66e03bb8d1e310VgnVCM10000071d60f89RCRD)

Non Regulated Lead Sample
-------------------------

The City provides a Residential Lead Testing Program free of charge to anyone
who wants to check their water. For some reason, the name is 2011-2014, but the
data actually goes up to 2016. Again, this is fairly geospatial, since you get
measurement and first three digits of postal code. However, since these are
unregulated and only measured when someone asks, it might be difficult to tease
out anything interesting.

See files in the [`Lead` directory](Lead).

ChemTrac
--------

Reports on usage of 25 "priority substances" from businesses since 2010. There's
an online API, but I just downloaded everything to the [`ChemTrac`
directory](ChemTrac).

 * `chemicals.csv`: List of 25 "priority substances"
 * `facilities.csv`: Information on businesses and facilities that are reporting
 * `chemical_use.csv`: Reports of usage since 2010

Street Tree Data
----------------

This is a pretty large dataset of trees within the City borders. I've only
included the [Readme](Street_Tree_Data_Readme.xls) because the dataset is ~40M.
It includes data on location, species and size. Again, this is a fairly
geospatial data set, but there might be something interesting there tying in
with neighbourhood age, urban development, etc.

Toronto Beaches Water Quality
-----------------------------

A "real-time" (aka, only in the summer) feed of E. coli readings at 11 of
Toronto's beaches. This can be found in the [`Beaches` directory](Beaches), with
instructions for the API in `Toronto_Beaches__Water_Quality_Readme.doc`. This
data ranges from 2007 to 2016, but the XML is pretty verbose. It includes
advisory text for every beach for every sample even when that advisory is the
same. So it will require a bit of data cleaning just to reduce that redundancy.


Ontario Open Datasets
=====================

Again, a lot of economic stuff and maps and such, but maybe a few things of
interest. All these datasets are licensed under the [Open Government
License](https://www.ontario.ca/page/open-government-licence-ontario).

[More datasets are available](https://www.ontario.ca/search/data-catalogue).

Air quality stations
--------------------

Data from the air monitoring station network, which is made up of continuous
pollutant monitors throughout the province.

This [one](https://www.ontario.ca/data/air-quality-stations) seems to be only
summarized, but there's the [whole hourly
dataset](https://www.ontario.ca/data/air-quality-monitoring-network) under
review. Hopefully, they'll be opening that up some time.

Drinking Water Surveillance Program
-----------------------------------

Provides water quality information at selected municipal drinking water systems
for scientific and research purposes.

This is pretty large, 1998-2012, so [check out the dataset
directly](https://www.ontario.ca/data/drinking-water-surveillance-program).

Energy use and greenhouse gas emissions for the Broader Public Sector
---------------------------------------------------------------------

Shows the amount of energy used and greenhouse gases (GHG) emitted for the
Broader Public Sector, i.e., municipalities, municipal service boards, school
boards, universities, colleges and hospitals.

Pretty large also, so [see online
dataset](https://www.ontario.ca/data/energy-use-and-greenhouse-gas-emissions-broader-public-sector)

Ontario Lake Partner
--------------------

Provides total phosphorus concentrations and water transparency.

 * [phosphorus](LPP/Lake_Partners1.csv)
 * [calcium](LPP/Lake_Partners2.csv)
 * [water transparency](LPP/Lake_Partners3.csv)

See [info](https://www.ontario.ca/data/ontario-lake-partner) and the [map of
collection
locations](https://www.ontario.ca/environment-and-energy/map-lake-partner).

Monitoring Studies
------------------

Multiple data sets about insecticides, pesticides, etc.

* [Benthic Invertebrate Neonicotinoid Monitoring
   Study](https://www.ontario.ca/data/benthic-invertebrate-neonicotinoid-monitoring-study)
* [Bumble Bee Diversity and Abundance
   Survey](https://www.ontario.ca/data/bumble-bee-diversity-and-abundance-survey)
* [Drinking Water Neonicotinoid Monitoring
   Study](https://www.ontario.ca/data/drinking-water-neonicotinoid-monitoring-study)
* [Pollen Monitoring Network
   Study](https://www.ontario.ca/data/pollen-monitoring-network-study)
* [Stream Neonicotinoid Monitoring
   Study](https://www.ontario.ca/data/stream-neonicotinoid-monitoring-study)
* [Soil Neonicotinoid Monitoring
   Study](https://www.ontario.ca/data/soil-neonicotinoid-monitoring-study)

Provincial (Stream) Water Quality Monitoring Network
----------------------------------------------------

https://www.ontario.ca/data/provincial-stream-water-quality-monitoring-network

Provides stream water quality monitoring data for a number of parameters
including chloride, nutrients and metals.

Water chemistry (Great Lakes nearshore areas)
---------------------------------------------

This dataset contains information on water quality samples collected from
nearshore stations within a lake basin.

The data is a pretty large Excel file, so [go directly to the
dataset](https://www.ontario.ca/data/water-chemistry-great-lakes-nearshore-areas).
