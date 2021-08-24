

* Clarify and agree on the scope of the system
* User cases (description of sequences of events that, taken together, lead to a system doing something useful)
    * Who is going to use it?
    * How are they going to use it?
* Constraints
    * Avaialabilty/Reliability/SLA
    * Mainly identify traffic and data handling constraints at scale.
    * Scale of the system such as requests per second, requests types, data written per second, data read per second)
    * Special system requirements such as multi-threading, read or write oriented.

### Start designing

* High level architecture design (Abstract design)
    Sketch the important components and connections between them, but don't go into some details.
    Application service layer (serves the requests)
    List different services required.
    Data Storage layer
    eg. Usually a scalable system includes webserver (load balancer), service (service partition), database (master/slave database cluster) and caching systems.
* Component Design
    Component + specific APIs required for each of them.
    Object oriented design for functionalities.
        Map features to modules: One scenario for one module.
        Consider the relationships among modules:
            Certain functions must have unique instance (Singletons)
            Core object can be made up of many other objects (composition).
    One object is another object (inheritance)
* Database schema design.
  * model DB
  * tables required and the schema
  * indexes(primary, secondary)
* Understanding Bottlenecks
    Perhaps your system needs a load balancer and many machines behind it to handle the user requests. * Or maybe the data is so huge that you need to distribute your database on multiple machines. What are some of the downsides that occur from doing that?
    Is the database too slow and does it need some in-memory caching?
* Scaling your abstract design