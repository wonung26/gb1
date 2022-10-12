# Managers

### Different approaches of scalability[#](broken-reference) <a href="#different-approaches-of-scalability" id="different-approaches-of-scalability"></a>

Here are the different ways to implement scalability.

#### Vertical scalability—scaling up[#](broken-reference) <a href="#vertical-scalability-scaling-up" id="vertical-scalability-scaling-up"></a>

**Vertical scaling**, also known as “**scaling up**,” refers to scaling by providing additional capabilities (for example, additional CPUs or RAM) to an existing device. Vertical scaling allows us to expand our present hardware or software capacity, but we can only grow it to the limitations of our server. The dollar cost of vertical scaling is usually high because we might need exotic components to scale up.

#### Horizontal scalability—scaling out[#](broken-reference) <a href="#horizontal-scalability-scaling-out" id="horizontal-scalability-scaling-out"></a>

**Horizontal scaling**, also known as “**scaling out**,” refers to increasing the number of machines in the network. We use commodity nodes for this purpose because of their attractive dollar-cost benefits. The catch here is that we need to build a system such that many nodes could collectively work as if we had a single, huge server.
