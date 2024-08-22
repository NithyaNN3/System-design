## Reliability
- **Tolerant of 'faults'**: Works as expected even under unexpected conditions
- Failures are not the same as faults. Failures are when the system fails to provide a service itself.
- Hardware faults (like disk death, redundancy), Software errors (like slow service, software bugs), Human errors (like config errors) 

## Scalability
- Ability to cope with increased load
- What is load? No. of requests to a server, ratio of reads to writes on database, simultaneous users in a chatroom, etc.
- Load affects performance of a system
- **throughput** - no. of records we can run in a second or total time it takes to run a job on a dataset
- **service time** - amount of time to process a request
- **response time** - service time + queue time, network delays
- **Handling load** - _Vertical scaling:_ shifting to more powerful machines; _Horizontal scaling:_ distributing the load onto several machines
- **Elasticity** refers to a systems that detect load increase and add computing resources
- Scaling introduces complexity and sometimes, lesser control. Preferred when there is predictability.

## Maintainability
- Follows convention, standard that can be understood by future devs
- Maintaining could be fixing bugs, maintaining operability, fixing failures, modification to new use cases
- 

