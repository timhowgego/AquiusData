# Spanish Railways

## About

### All Operators, Friday 20 July 2018

Snapshot of all non-tourist passenger train services within Spain. See [Disassembling Trenes](https://timhowgego.wordpress.com/2018/09/04/disassembling-trenes/) for more information about the original research behind this dataset.

### Renfe LD/MD, 10-16 December 2018

Renfe Operadora [GTFS extract](http://data.renfe.com/), excluding Cercanías, Feve, Trenhotel and non-domestic services.

## Live Demonstrations

* [Spanish Railways (Friday 20 July 2018)](https://timhowgego.github.io/Aquius/live/es-rail-20-jul-2018/)
* [Renfe Obligación de Servicio Público (Friday 20 July 2018)](https://timhowgego.github.io/Aquius/live/renfe-osp-20-jul-2018/)
* [Renfe LD/MD (10-16 December 2018)](https://timhowgego.github.io/Aquius/live/renfe-ld-md-dec-2018/)

## Known Issues

Services are not totally accurate: The 20 July 2018 network was research in one direction (away from Madrid), during academic holidays, and with a Cercanías journey planner that only showed origin/destination and not the stops inbetween. Likewise service totals for many city metros were calculated from average headways, so won't be perfectly accurate. Tourist-type services have been excluded. International services only within Spain. For an introduction to the dataset, see [Disassembling Trenes](https://timhowgego.wordpress.com/2018/09/04/disassembling-trenes/).

Certain circular services are summarised incorrectly: Madrid's C-7 at Atocha is a specific exception to the rule that circular services are counted just once, because each C-7 loop serves different stations, and consequently the count of trains specifically at Atocha (the total arrival/departure in all directions) differs from the count of trains in the bottom-left panel (the total number of unique services involved). The Parla tram, which is both circular and differs by direction, is counted in both directions since because its unequal frequencies make it difficult to determine which direction will get to any one destination fastest.

Time periods are inaccurate: The time periods included in the Renfe LD/MD dataset are assigned from the average of each train journey's start (at origin) and end (at final destination) time. Long distance journeys may operate over many hours. For example, a train that starts at 11:00 and travels for 3 hours until 14:00 is, on average, an afternoon train. These time periods should be used only as a broad indicator of the spread of services throughout the day, not a precise guide.

## License

The Spanish Railway dataset is a creative work of academic curiosity, a limited snapshot of one moment in history. The original creator makes no claim of ownership to any data therein, nor should be held responsible for its accuracy. Such can therefore be used as "freely" as its source. Population data is "Prepared with data extracted from the INE website: [www.ine.es](http://www.ine.es/)", apparently with no restriction on reuse beyond that statement. Municipality centroids CC BY 4.0 from [Instituto Geográfico Nacional de España](http://www.ign.es/). National network station nodes were originally from the [IDEAADIF](http://ideadif.adif.es/) (INSPIRE) dataset, apparently under the same license. 20 July 2018 operator data was researched from operator websites. Later [Renfe open data](http://data.renfe.com/legal), "Origen de los datos: Renfe Operadora".