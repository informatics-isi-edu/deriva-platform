# DERIVA Platform

The Discovery Environment for Relational Information and Versioned Assets (DERIVA) platform is an asset management system designed to support scientific collaboration through the full lifecycle of data - from early experiment design, to data acquisition, analyses and ultimately publication.

The following technologies developed at the Informatics Systems Research division of ISI/USC form the ecosystem that supports DERIVA's features. You can find documentation for these components at [https://docs.derivacloud.org/](https://docs.derivacloud.org/):

* Multi-tenant relational data service for domain models ([ERMrest](https://github.com/informatics-isi-edu/ermrest)) with a client library ([ERMrest JS](https://github.com/informatics-isi-edu/ermrestjs)) and python modules (which include [DERIVA PY](https://github.com/informatics-isi-edu/deriva-py) and [DERIVA QT](https://github.com/informatics-isi-edu/deriva-qt)),
* Object storage service for assets ([HATRAC](https://github.com/informatics-isi-edu/hatrac)),
* Suite of adaptive user interface applications ([CHAISE](https://github.com/informatics-isi-edu/chaise)),
* Suite of utilities for ingest and export of assets and metadata ([IObox](https://github.com/informatics-isi-edu/iobox)),
* Asset aggregation package format ([BDBag](https://github.com/ini-bdds/bdbag)), and
* Shared authentication layer ([WebAuthN](https://github.com/informatics-isi-edu/webauthn))

**ERMrest**: (rhymes with "earn rest") General relational data storage service for web-based, data-oriented collaboration. It allows general entity-relationship modeling of data resources manipulated by RESTful access methods. A client library - ERMrest JS - is also available.
Git Repo: [https://github.com/informatics-isi-edu/ermrest](https://github.com/informatics-isi-edu/ermrest)

**ERMrest JS**: Javascript client library for accessing ERMrest services and HATRAC services.
Git Repo: [https://github.com/informatics-isi-edu/ermrestjs](https://github.com/informatics-isi-edu/ermrestjs)

**DERIVA PY**: Python modules for accessing ERMrest and HATRAC services.
Git Repo: [https://github.com/informatics-isi-edu/deriva-py](https://github.com/informatics-isi-edu/deriva-py)

**DERIVA QT**: Python modules for graphical user interface tools such as Authentication and File Upload.
Git Repo: [https://github.com/informatics-isi-edu/deriva-qt](https://github.com/informatics-isi-edu/deriva-qt)

**HATRAC**: (pronounced "hat rack") Simple object storage service for web-based, data-oriented collaboration. It presents a simple HTTP RESTful service model with hierarchical data naming, access control suitable for collaboration, trivial support for browser-based applications, referential stability for immutable data, atomic binding of names to data and consistent use of distributed data.
Git Repo: [https://github.com/informatics-isi-edu/hatrac](https://github.com/informatics-isi-edu/hatrac)

**CHAISE**: Model-driven web interface (more formally a user agent) for data discovery, analysis, visualization, editing, sharing and collaboration over tabular data (more specifically relational data) served up as Web resources by the ERMrest service. CHAISE dynamically renders relational data resources based on a small set of baseline assumptions, combined with its rendering heuristics, and finally user preferences in order to support common user interactions with the data. CHAISE is developed in JavaScript, HTML, CSS, and runs in most modern Web browsers. It is the front-end component of the suite of tools including ERMrest, HATRAC, and IObox.
Git Repo: [https://github.com/informatics-isi-edu/chaise](https://github.com/informatics-isi-edu/chaise)

**IOBox**: Collection of Extract, Transform, Load (ETL) utilities for ERMrest+Hatrac. Extract: Connects to a data source (or read from a file) and generates a data "bag". Transform: Takes a "bag", runs transformations and outputs an updated "bag". Load: Takes a "bag" and loads it into a data sink.
Git Repo: [https://github.com/informatics-isi-edu/iobox](https://github.com/informatics-isi-edu/iobox)

**BDBag**: Used with IOBox (see above). Specification for asset aggregation packages - simple yet powerful mechanisms for specifying, sharing, and managing complex, distributed, large datasets - or “bags”. These combine a simple and robust method for describing data collections (BDBags), data descriptions (Research Objects), and simple persistent "minimal identifiers" (Minids) to create a powerful ecosystem of tools and services for big data analysis and sharing.
Git Repo: [https://github.com/ini-bdds/bdbag](https://github.com/ini-bdds/bdbag)

**WebAuthN**: Compact, modular authentication provider framework written to support Python-based, RESTful Web services and is used by ERMrest and HATRAC. It allows deployment-time configuration of several alternative identity and attribute provider modules to establish client security contexts for Web requests by talking to a local or remote provider.
Git Repo: [https://github.com/informatics-isi-edu/webauthn](https://github.com/informatics-isi-edu/webauthn)

*DERIVA has been funded by the National Institute of Health (NIH) via grants 5U24DK110814, 1U01DK107350, 5U01DE024449, 5R01MH107238, 5U54EB020406, P41-EB015922 and the GPCR Consortium.*
