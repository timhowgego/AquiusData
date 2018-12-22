# FlixBus

## About

The FlixBus network is almost impossible to communicate on a fixed map because its service patterns are often defined by cabotage restrictions, especially in Iberia and the Balkans. Such cabotage restrictions may prevent FlixBus conveying passengers _within_ countries or regions, often rendering the destinations available to passengers quite different to the route taken by the vehicle. This added complexity is not a limitation for [Aquius](https://timhowgego.github.io/Aquius/), which always draws its route map from a user-specified _here_.

FlixBus represents an extreme test case for this style of operation, since on some routes almost every place served is defined with a different set of boarding and alighting restrictions. FlixBus [host their own dynamic network map](https://www.flixbus.co.uk/bus-routes), however this can feel laggy, and does not give any indication of service frequency - destinations with one bus a week are shown just as prominantly as destinations with one bus an hour. The Aquius dataset is relatively large - almost 1 MegaByte uncompressed, even without headcode information and day-by-day service filters (which can potentially be [built from GTFS](https://timhowgego.github.io/Aquius/live/gtfs/)) - but is smoother to use and more indicative of services.

[FlixMobility GmbH](https://www.flixbus.de/) has rapidly grown to become the most dominant international (and to a lesser degree, inter-regional) bus operator in Europe. The FlixBus network started to stabilise by 2018. August represents the network at or near its full extent, including summer seasonal routes. The population data is regional, indicative of the approximate catchment of international services. In most cases European NUTS level 2 data has been used as is. In a few cases (such as inner and outer London, or Berlin and Brandenburg) NUTS 2 zones that originally separated large cities from their immediate hinterlands have been merged together.

## Live Demonstrations

* [FlixBus (20-26 August 2018](https://timhowgego.github.io/Aquius/live/flixbus-aug-2018/)

## License

The FlixBus dataset is a creative work of academic curiosity, a limited snapshot of one week in history. The original creator makes no claim of ownership to any data therein, nor should be held responsible for its accuracy. Such can therefore be used as "freely" as its source:

* FlixBus GTFS is hosted by [NDOV Loket](https://ndovloket.nl/) as "Open Data". Officially FlixBus offer their GTFS data [only to affiliate partners](https://global.flixbus.com/company/partners/affiliate-partners).
* [https://ec.europa.eu/eurostat/about/policies/copyrightEurostat](https://ec.europa.eu/eurostat/about/policies/copyright) populatstion statsitics are freely reusable with attribution.
