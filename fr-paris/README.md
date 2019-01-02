# Paris

## About

The dataset contains a one week snapshot of every scheduled public transport service within the Petite Couronne of Paris: The City and its immediate suburbs (Hauts-de-Seine, Seine-Saint-Denis, and Val-de-Marne) - Departments 75, 92, 93 and 94. Paris is one of the most populous urban areas in Europe, while the City herself contains some of the most densely populated areas of Europe - both conditions that engender a large public transport network. The urban area of Paris sprawls into the wider Île-de-France region, especially along the Seine valley. The transport networks in these outer areas tend to focus on local centres, and are sometimes quite rural in character, thus in most cases (RER commuter rail is the main exception) these areas should not reasonably be considered part of the Parisian network.

The underlying network data is that maintained by [Île-de-France Mobilités as GTFS](https://opendata.stif.info/explore/dataset/offre-horaires-tc-gtfs-idf/information/). The featured Petite Couronne network is dominated by Parisian state operator RATP (metro, most bus, most tram, and some rail), although state railway operator SNCF is also significant (primarily as RER), and various smaller operators also provide limited local bus services, especially in the periphery.

Paris has a specific night-bus operation called Noctilien, which has been isolated to allow easier analysis of day and night networks. Networks are otherwise summarised only by day of week. Service levels do vary across the day (tending to peak at around 08:30 and 18:00), but these variations are generally affected by changes in route headway, not the introduction of new or different peak routes. Consequently the peak network tends to look similar to that found during the day. The network has been built without stop/station names to minimise filesize (names would otherwise double the filesize).

Population is that in 2013, shown by Insee "Grand Quartier" - an intermediate geography, larger than the base IRIS areas, but (in most urban cases) smaller than Communes. Grand Quartiers vary greatly in population (within the Petite Couronne of Paris, between 1 and 100 thousand people), but their scale correlates better to nature local public transport catchment areas. Grand Quartier are often divided by principle roads and thus the allocation of stops on either side of the road (to one Quartier or another) can result in quirks, such as the same overall bus service being assigned to different Quartier in different directions. Overall such quirks tend to average out, but care should be taken when investigating very specific routes or single Grand Quartier.

**Caution:** The Parisian public transport network rarely changes from week-to-week, and only selectively changes from year-to-year, so long after January 2019 this network snapshot is likely to look _similar_ to some future network. However, such a snapshot should not be used if current accuracy is important. The snapshot should not be used to plan an actual journey. And certainly not without checking the results against current operator/agency publicity.

## Live Demonstrations

* [Inner Paris (7-13 January 2019)](https://timhowgego.github.io/Aquius/live/petite-paris-2019/)

## Of Interest

* [La Défense Daytime](https://timhowgego.github.io/Aquius/live/petite-paris-2019/#x2.28/y48.8907/z12/c2.24224/k48.88989/m13/n1) - the modern commercial core, devoid of direct links to much of the City of Paris' population, in spite of its proximity.

## License

The dataset is a creative work of academic curiosity, a limited snapshot of one week in history. The original creator makes no claim of ownership to any data therein, nor should be held responsible for its accuracy. Such can therefore be used as "freely" as its source:

* [Île-de-France Mobilités](https://opendata.stif.info/explore/dataset/offre-horaires-tc-gtfs-idf/information/) (stops and services) - [Open Database License v1.0](http://vvlibri.org/fr/licence/odbl-10/legalcode/unofficial).
* [Insee](https://www.insee.fr/fr/information/2381863) (2013 population) - unrestricted reused.

