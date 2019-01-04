# United Kingdom Rail

## About

The Great Britain National Rail dataset is a snapshot of all weekday passenger train service patterns across [Network Rail](https://www.networkrail.co.uk/), except (international) Eurostar. A small number of bus and ferry routes are included where these are traditionally considered part of the railway network, such as Heathrow-Woking. Links are organised and coloured by train operating company.

The dataset has been built from the [Planar Network's GTFS](https://planar.network/projects/feeds), and makes extensive use of dummy waypoints to show the route taken by trains, regardless of their stops. This results in a relatively neat map where service totals at stations are not automatically the same as the sum of the links passing those stations.

Population is by District (or Unitary Authority equivalent), using [2017 population estimates](https://www.ons.gov.uk/peoplepopulationandcommunity/populationandmigration/populationestimates/datasets/populationestimatesforukenglandandwalesscotlandandnorthernireland). Districts are a geographic compromise - too crude to properly analyse urban networks, and too detailed to analyse a whole nation - but overall they give a broad indicator of the people served.

**Caution:** The railway network rarely changes from week-to-week, and only selectively changes from year-to-year, so long after January 2019 this network snapshot is likely to look _similar_ to some future network. However, such a snapshot should not be used if current accuracy is important. The snapshot should not be used to plan an actual journey. And certainly not without checking the results against current operator/agency publicity.

## Live Demonstrations

* [Great Britain National Rail (weekdays, January 2019)](https://timhowgego.github.io/Aquius/live/gb-rail-2019/)

## Known Issues

Merseyrail lasso routes round the central Liverpool city loop may display the full train journey, both out and back, and thus may appear to duplicate service counts.

Dummy waypoints may cause erroneous miscalculation of totals on links immediate after _here_, where the first node of that link is a waypoint and only one node on the entire link is within _here_. Node totals remain correct - the error lay in link rendering.

## License

The Great Britain National Rail dataset is a creative work of academic curiosity, a limited snapshot of one moment in history. The original creator makes no claim of ownership to any data therein, nor should be held responsible for its accuracy. Such can therefore be used as "freely" as its source:

* [Office of National Statistics](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/) - Open Government Licence.
* [Rail Delivery Group](http://data.atoc.org/licence-restrictions) - use "for your own business purposes", with attribution to [RSP](https://www.raildeliverygroup.com/). RSP's data has been processed via a GTFS archive created by the [Planar Network](https://planar.network/projects/feeds).
