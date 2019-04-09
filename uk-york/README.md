# City of York

## About

Snapshot of all bus services within the City of York. York is a centrally-focused small city network with one dominant urban operator (First York), augmented by several minor local operators, and inter-urban operators. Bus is the only significant public transport mode within the city: York-Poppleton is the only railway station pairing - its services are not included in the Aquius dataset.

York's network is characterised by six large edge-of-town "Park and Ride" sites, where rural travellers transfer from private car to public bus for journeys into the centre. The busiest single bus corridor, that to the university on the south-east side of the city, is notable in connecting only to the centre of York.

The dataset has been created by [converting TransXchange files](https://github.com/planarnetwork/transxchange2gtfs) for the Yorkshire region into GTFS, then [GTFS into Aquius](https://timhowgego.github.io/Aquius/live/gtfs/). TransXchange is the standard datamodel for administering bus service registrations in Great Britain, but lacks much user-friendly information, such as familiar routes names, colours and website links. Those customisations where added via the GTFS processing configuration.

**Caution:** The York public transport network rarely changes from week-to-week, and only selectively changes from year-to-year, so long after April 2019 this network snapshot is likely to look _similar_ to some future network. However, such a snapshot should not be used if current accuracy is important. The snapshot should not be used to plan an actual journey. And certainly not without checking the results against current operator/agency publicity.

## Live Demonstrations

* [York (2019)](https://timhowgego.github.io/Aquius/live/york-2019/)

## Known Issues

The dedicated university shuttle service (UB1) is missing, since it does not appear in the Traveline dataset.

## License

The City of York dataset is a creative work of academic curiosity, a limited snapshot of one moment in history. The original creator makes no claim of ownership to any data therein, nor should be held responsible for its accuracy. Such can therefore be used as "freely" as its source. Both sources are reusable with attribution, under an [Open Government Licence](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/):

* [Office of National Statistics](https://www.ons.gov.uk/census/2011census/) - 2011 Ward census population.
* [Traveline National Dataset](https://www.travelinedata.org.uk/traveline-open-data/traveline-national-dataset/) - services and stops.
