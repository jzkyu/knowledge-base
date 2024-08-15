A group of tasks ([[task]]) is *deadlocked* if each task in the group is waiting for an event that only another task in the group can trigger.

None of the tasks can run, release resources, or be awakened.

See: Philosopher table example. 

A *deadlock* is the ultimate stage of [[starvation]]. 

Characteristics:
- Mutual exclusion / bounded resources
- Hold and wait
- No preemption
- Circular wait

Strategies:
- Ostrich algorithm
	- Mitigation: Make it less painful for users
- Detection and recovery
- Dynamic avoidance; careful resource allocation
- Prevention; negating one of the conditions