# Scalability
* The capability of system, process, or network to grow and manage increased demand
* Any distributed system that can continuously evolve in order to support the growing amount of work is considered to be scalable

### Problem
* The performance of a system (despite designed or claimed to be scalable) declines with the system size due to:
  * management
  * environment cost

### Reasons for scaling
* Increased data volume
* Increased amount of work (e.g. number of transactions)

### Goal
* Achieve scaling without performance loss

### Example:
* Network speed may become slower because machines tend to be far apart from one another
* Some tasks may not be distributed. Possible reasons:
  * Their inherent atomic nature
  * A flaw in the system design
* At some point, such tasks can limit the speed-up obtained by distribution
* A scalable architecture avoids this situation and attempts to balance the load on all the participating nodes evenly

## Solutions

### Horizontal vs. Vertical Scaling
Vertical scaling:
* Scale by adding more power (CPU, RAM, Storage, etc.) to an existing server
* Usually limited to the capacity of a single server
* Scaling beyond the current capacity involves downtime and comes with an upper limit
* Example:
  * MySQL
    * Allows for an easy way to scale vertically by switching from smaller to bigger machines

Horizontal scaling:
* Add more servers into your pool of resources
* Easier to scale dynamically by adding more machines
* Examples:
  * [Cassandra](https://en.wikipedia.org/wiki/Apache_Cassandra) & [MongoDB](https://en.wikipedia.org/wiki/MongoDB)
    * They provide an easy way to scale horizontally by adding more machines to meet growing needs
