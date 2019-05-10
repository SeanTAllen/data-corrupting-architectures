# Data Corrupting Architectures We Know and Love

## Abstract

There’s an old distributed systems adage, “You can have a second computer when you learn how to use the first one.” When it comes to data-access patterns, most of our favorite patterns are unsafe on a single computer. Most of our applications assume a concurrency model where all access is serialized. What happens when that mental model meets distributed data?

Sean Allen reviews data race and corruption problems that exist on single-machine systems and shows how we’ve transferred many of those patterns over to distributed systems and distributed state. You’ll learn the basics of data races, deadlocks, and problems in even the simplest of our concurrent data access patterns and how our existing scaling patterns replicate the same issues across multiple machines, increasing the potential problems, as well as designs that can alleviate them.

## Versions of this talk

* ScaleConf Colombia 2019
* VelocityConf San Jose 2019

## References

* [Actor Model](https://en.wikipedia.org/wiki/Actor_model)
* [CRDT Primer](http://jtfmumm.com/blog/2015/11/17/crdt-primer-1-defanging-order-theory/)
* [Data Race](https://doc.rust-lang.org/nomicon/races.html)
* [Event Sourcing](https://www.martinfowler.com/eaaDev/EventSourcing.html)
* [Linearizability](https://en.wikipedia.org/wiki/Linearizability)
* [Locks and Mutexes](https://en.wikipedia.org/wiki/Lock_(computer_science))
* [Synchronization](https://en.wikipedia.org/wiki/Synchronization_(computer_science))

## Additional References

* [Jepsen: Riak](https://aphyr.com/posts/285-jepsen-riak)
* [Lasp: A Language for Distributed, Eventually Consistent Computations with CRDTs](https://www.info.ucl.ac.be/~pvr/papoc-2015-lasp-abstract.pdf)
* [Rich Hickey: Deconstructing the Database](https://www.youtube.com/watch?v=Cym4TZwTCNU)
* [There is No Now](https://queue.acm.org/detail.cfm?id=2745385)
