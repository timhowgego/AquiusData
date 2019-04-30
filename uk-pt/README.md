# United Kingdom Public Transport

## About

The Great Britain Terrestrial Public Transport dataset contains a snapshot of every scheduled weekday public transport service operating within Great Britain, except aviation. The territory excludes (Northern) Ireland, the Isle of Man and the Channel Islands.

Data is sourced regionally from Traveline, and nationally from the Coach Database and Rail Delivery Group. Services included reflect those sources. Scheduled services primarily aimed at tourists (such as preserved railway lines) are generally included, but not always. Semi-scheduled Demand Responsive Services are typically included by showing all possible journey options, and thus may over-represent actual operations.

Service level is summarised as an average weekday. Most local bus routes operate the same service pattern on each weekday. Where a service operates on, for example, just one day, this is expressed as 0.2 of a daily service.

Rather than display individual stops, service are shown as links between the areas they serve: In the first instance, between electoral Wards. Ward geography broadly reflects the scale of local public transport, while still relating services to local notions of place. In urban areas Wards broadly match walking catchments. In rural areas such catchments are may be affected by car. Wards may be considered too large to be meaningful in areas with especially low population density, notably north-west Scotland, where the map needs to be analysed with caution. Wards do not reflect the catchment of longer distance services. Districts better reflect mid distance travel.

Each service included must stop at least once within the area's boundaries. Services that only serve the area itself are excluded (connectivity analysis assumes each area has perfect connectivity within itself). Only the centroid of each area is mapped. Services that cross the same boundary between areas more than once are counted more than once between those areas. This is intentional, since those services do provide multiple links across the boundary.

Data can be filtered by mode or operating group. Each operating company is assigned to one mode, but such an allocation is not always perfect: For example, rail operators may sponsor replacement bus services, while Community Transport operators may provide both scheduled and semi-scheduled services. But broadly: Rail includes heavy rail, metro, tram and Underground. Bus excludes operators of Demand Responsive and taxi-like services.

Groups are based on Traveline's NOC database, ammended for known errors. Join ventures are attributed to the most dominant partner. There are four large "British" (in origin) groups: Arriva, First and Go-Ahead, each providing about 13% of all services, and Stagecoach providing 20%. Other British Groups include Centrebus, National Express, Rotala, Serco and Wellglade. Notable Overseas Groups are Abellio, ComfortDelgro, RATP and Transdev, among others. The State includes only direct operations by government (not franchises or concessions) - national (LNER) and local (TfL) rail, traditional municipal city operations (such as Lothian), and specific council bus routes (primarily rural).

The sample period, the first week of April 2019, was during school term time, the week immediately before the Easter holidays. The period excluded summer-only routes and some university services, but is otherwise "typical".

Population is that [estimated in mid-2017](https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates/datasets/wardlevelmidyearpopulationestimatesexperimental). Traveline archives have been processed using [transxchange2gtfs](https://github.com/planarnetwork/transxchange2gtfs).

**Caution:** Long after April 2019 this network snapshot is likely to look _similar_ to some future network. However, such a snapshot should not be used if current accuracy is important. The snapshot should not be used to plan an actual journey. And certainly not without checking the results against current operator/agency publicity.

## Live Demonstrations

* [GB by Ward (2019)](https://timhowgego.github.io/Aquius/live/gb-pt-ward-2019/)
* [GB by District (2019)](https://timhowgego.github.io/Aquius/live/gb-pt-district-2019/)

## Known Issues

Longer-distance local services operated by the same vehicle throughout may be broken into two or more route segments. Examples include many longer distance Stagecoach services, such as those via Ellon, X5 Oxford-Cambridge, and Bude-Barnstaple. These are quirks of the underlying Traveline data, perhaps intended to allow services to be allocated within local government boundaries, but actually making such through journey opportunities invisible to many intending travellers: Both Google and Traveline journey planners currently fail to find through journeys, since the link between fragmented routes cannot be reliably established without specific local knowledge. Note that advertised connections between different routes are treated separately by design.

Services across regional borders may be double counted. The underlying data is sourced regionally, and while inter-regional services are theoretically assigned to just one regional dataset, in practice a few services were found to be duplicated in both sources - mostly from the north of England. Known errors have been corrected, but it is entirely likely that a few duplicates are still lurking.

Buses that use vehicle ferries may double-count the connection across the water. In practice there is only one known case in the dataset, on the far north of the Shetlands. Plymouth's Torpoint ferry is not included individually in the original Traveline data, and thus there is no duplication with the buses it conveys. This quirk is not readily fixable, since buses on ferries generally use slightly different stops and times to the ferry itself.

Joint operations of single routes (for example, Arriva/Stagecoach 685 Newcastle-Carlisle) are attributed to the dominant operator unless filtered by operating group. Filtering by group should correctly split such services.

Specific services are missing. These typically reflect ommissions in the Traveline data. Of particular note, service changes around Lowesoft at the start of April have resulted in services disappearing entirely - such as the 99 to Lowesoft-Southwold, the most frequent route from Southwold.

Demand Responsive Transport service patterns are visually hapzard. Again, this reflects the Traveline data, where each service is assigned to every orgin/destination it might serve, depending on user requests.

The allocation of stops to Wards and Districts uses a rounded coordinate precision, which may incorrectly assign stops that are located very close to boundaries. In practice stops so close any boundary will serve more than one area, and thus their allocation is already somewhat arbitary.

## License

The Great Britain Terrestrial Public Transport dataset is a creative work of academic curiosity, a limited snapshot of one moment in history. The original creator makes no claim of ownership to any data therein, nor should be held responsible for its accuracy. Such can therefore be used as "freely" as its source:

* [Office of National Statistics](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) - Open Government Licence.
* [Rail Delivery Group](http://data.atoc.org/licence-restrictions) - use "for your own business purposes", with attribution to [RSP](https://www.raildeliverygroup.com/). RSP's data has been processed via a GTFS archive created by the [Planar Network](https://planar.network/projects/feeds).
* [Traveline National Dataset](https://www.travelinedata.org.uk/traveline-open-data/traveline-national-dataset/) - Open Government Licence.
