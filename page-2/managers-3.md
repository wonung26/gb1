# Managers

Let’s discuss some important features for which fault-tolerance becomes a necessity.

Availability focuses on receiving every client’s request by being accessible 24/7.

Reliability is concerned with responding by taking specified action on every client’s request.

#### Fault tolerance techniques[#](broken-reference) <a href="#fault-tolerance-techniques" id="fault-tolerance-techniques"></a>

Failure occurs at the hardware or software level, which eventually affects the data. Fault tolerance can be achieved by many approaches, considering the system structure. Let’s discuss the techniques that are significant and suitable for most designs.

**Replication**[**#**](broken-reference)

One of the most widely-used techniques is **replication-based fault tolerance**. With this technique, we can replicate both the services and data. We can swap out failed nodes with healthy ones and a failed data store with its replica. A large service can transparently make the switch without impacting the end customers.

We create multiple copies of our data in separate storage. All copies need to update regularly for consistency when any update occurs in the data. Updating data in replicas is a challenging job. When a system needs strong consistency, we can synchronously update data in replicas. However, this reduces the availability of the system. We can also asynchronously update data in replicas when we can tolerate eventual consistency, resulting in stale reads until all replicas converge. Thus, there is a trade-off between both consistency approaches. We compromise either on availability or on consistency under failures—a reality that is outlined in the [CAP theorem](https://www.educative.io/edpresso/what-is-the-cap-theorem).
