# Data Corrupting Architectures We Know and Love

## Abstract

There’s an old distributed systems adage, “You can have a second computer when you learn how to use the first one.” When it comes to data-access patterns, most of our favorite patterns are unsafe on a single computer. Most of our applications assume a concurrency model where all access is serialized. What happens when that mental model meets distributed data?

Sean Allen reviews data race and corruption problems that exist on single-machine systems and shows how we’ve transferred many of those patterns over to distributed systems and distributed state. You’ll learn the basics of data races, deadlocks, and problems in even the simplest of our concurrent data access patterns and how our existing scaling patterns replicate the same issues across multiple machines, increasing the potential problems, as well as designs that can alleviate them.

## Versions of this talk

* ScaleConf Colombia 2019
* VelocityConf San Jose 2019

## References

* [Actor Model](https://en.wikipedia.org/wiki/Actor_model)
* [Atomicity](https://en.wikipedia.org/wiki/Atomicity_(database_systems))
* [Concurrency](https://en.wikipedia.org/wiki/Concurrency_(computer_science))
* [Consensus](https://en.wikipedia.org/wiki/Consensus_(computer_science))
* [CQRS](https://martinfowler.com/bliki/CQRS.html)
* [Conflict-free replicated data type (CRDT)](https://en.wikipedia.org/wiki/Conflict-free_replicated_data_type)
* [Data Race](https://doc.rust-lang.org/nomicon/races.html)
* [Distributed Transaction](https://en.wikipedia.org/wiki/Distributed_transaction)
* [Event Sourcing](https://www.martinfowler.com/eaaDev/EventSourcing.html)
* [Functions as a service](https://en.wikipedia.org/wiki/Function_as_a_service)
* [Linearizability](https://en.wikipedia.org/wiki/Linearizability)
* [Locks and Mutexes](https://en.wikipedia.org/wiki/Lock_(computer_science))
* [Paxos Consensus Algorithm](https://en.wikipedia.org/wiki/Paxos_(computer_science))
* [Raft Consensus Algorithm](https://raft.github.io/)
* [Serverless Architectures](https://martinfowler.com/articles/serverless.html)
* [Service statelessness principle](https://en.wikipedia.org/wiki/Service_statelessness_principle)
* [Shared-nothing Architecture](https://en.wikipedia.org/wiki/Shared-nothing_architecture)
* [Synchronization](https://en.wikipedia.org/wiki/Synchronization_(computer_science))
* [Transaction](https://en.wikipedia.org/wiki/Database_transaction)

## Dive Deeper

* [CRDT Primer](http://jtfmumm.com/blog/2015/11/17/crdt-primer-1-defanging-order-theory/)
* [Jepsen: Riak](https://aphyr.com/posts/285-jepsen-riak)
* [Lasp: A Language for Distributed, Eventually Consistent Computations with CRDTs](https://www.info.ucl.ac.be/~pvr/papoc-2015-lasp-abstract.pdf)
* [Pat Helland and Me: How to build stateful distributed applications that can scale almost infinitely](https://github.com/SeanTAllen/pat-helland-and-me)
* [Rich Hickey: Deconstructing the Database](https://www.youtube.com/watch?v=Cym4TZwTCNU)
* [There is No Now](https://queue.acm.org/detail.cfm?id=2745385)
