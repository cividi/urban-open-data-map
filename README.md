# Urban (Open) Data
An effort to map out urban open data initiatives, providers and entities. In the spirit of the wonderful [WoBike](https://github.com/ubahnverleih/WoBike) list.

## Switzerland

### Linked Open Data

#### Geo Admin

The swiss geographical service is running a SPARQL-endpoint for currently three datasets:

- [swissBOUNDARIES 3D](https://ld.geo.admin.ch/data/swissBOUNDARIES3D)
- [Generalized borders G1](https://ld.geo.admin.ch/data/generalizedBordersG1)
- [Public transport stops](https://ld.geo.admin.ch/data/PublicTransportStops)

#### City of Zurich

The statistical office of Zurich publishes their data as linked open data and runs a SPARQL endpoint [since August 2018](https://data.stadt-zuerich.ch/dataset/stadt_zuerich_losd).

* [Available LoD datasets](https://ld.stadt-zuerich.ch/sparql/#query=PREFIX+qb%3A+%3Chttp%3A%2F%2Fpurl.org%2Flinked-data%2Fcube%23%3E%0APREFIX+rdfs%3A+%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0A%0ASELECT++%3Fdataset+(COUNT(*)+AS+%3Fcount)+%3Flabel+WHERE+%7B+GRAPH+%3Chttps%3A%2F%2Flinked.opendata.swiss%2Fgraph%2Fzh%2Fstatistics%3E+%7B%0A%0A+++%3Fdataset+a+qb%3ADataSet+%3B+%0A+++%09%09rdfs%3Alabel+%3Flabel+.+%0A++++%0A+++%23%3Fobs+a+qb%3AObservation+%3B%0A+++%3Fobs+%3Chttp%3A%2F%2Fpurl.org%2Flinked-data%2Fcube%23dataSet%3E+%3Fdataset+.%0A%0A%7D%7D+GROUP+BY+%3Fdataset+%3Flabel&contentTypeConstruct=text%2Fturtle&contentTypeSelect=application%2Fsparql-results%2Bjson&endpoint=https%3A%2F%2Fld.stadt-zuerich.ch%2Fquery&requestMethod=POST&tabTitle=Query&headers=%7B%7D&outputFormat=table)

[Detailed documentation](https://github.com/statistikstadtzuerich/documentation)

## Zettelkasten

Possible Domains to do research in
* Sensor data
 * Water temperatures (e.g. Aare Bot)
 * Air temperatures
* Orthophotos
* Amtliche Vermessung (e.g. Geodienste)
* 3D Stadtmodelle
  * Luucy
  *
* Mapping / Routing
 * swisstopo
 * OpenStreetMap
 * Here Maps
 * Google Maps
