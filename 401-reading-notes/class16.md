#  Serverless Functions

What is serverless?
- Serverless is a cloud computing execution model that 

. Automatically provisions the computing resources required to run application code on demand, or in response to a specific event;
. Automatically scales those resources up or down in response to increased or decreased demand;
. Automatically scales resources to zero when the application stops running. 

Serverless vs. FaaS (function as a service)

- Serverless and function as a service (FaaS) are often conflated. But FaaS is actually a subset of serverless - it's the compute paradigm central to serverless, wherein application code or containers run only in response to events or requests. Serverless includes FaaS plus all the other associated resources and cloud services and resources supporting the code - e.g. storage, databases, networks, API gateways, authentication - for which configuration, management and billing of services are invisible to the user.

Serverless pros and cons

Pros
1. serverless enables development teams to focus on writing code, not managing infrastructure. It gives developers much more time to innovate and optimize their front-end application functionality and business logic.
2. serverless customers pay for execution only. The meter starts when the request is made, and ends when execution finishes. Compare to the infrastructure as a service (IaaS) compute model, where customers pay for the virtual machines (VMs) and other resources required to run applications, from the time they provision those resources until the time the customer explicitly decommissions those resources.
3. Serverless is a polyglot environment, enabling developers to code in any language or framework - Java, Python, node.js - with which they're comfortable.
4. Serverless simplifies deployment and, in a larger sense, simplifies DevOps cycles, because developers don't have to describe infrastructure needed integrate, test, deliver and deploy code builds into production.
5. For certain workloads, such as ones that require parallel processing, serverless can be both faster and more cost-effective than other forms of compute.
6. Serverless application development platforms provide near-total visibility into system and user times, and can aggregate that information systematically.

Cons
1. Stable or predictable workloads: Because serverless scales up and down on demand in response to workload, it offers significant cost savings for spiky workloads. But it does not offer the same savings for workloads characterized by predictable, steady or long-running processes; in these cases a traditional server environment might be simpler and more cost-effective.

2. Cold starts: Because serverless architectures forgo long-running processes in favor of scaling up and down to zero, they also sometimes need to start up from zero to serve a new request. For certain applications, this startup latency isn’t noticeable or detrimental to users. But for others - for example, financial trading application - the delay is unacceptable.

3. Monitoring and debugging: These operational tasks are challenging in any distributed system, but a move serverless architecture (or microservices architecture, or a combination of the two) only exacerbates the complexity. For example, teams may find it difficult or impossible to monitor or debug serverless functions using existing tools or processes.

4. Vendor lock-in: Serverless architectures are designed to take advantage of an ecosystem of managed cloud services and, in terms of architectural models, go the furthest to decouple a workload from something more portable, like a virtual machine (VM) or Docker container. For some companies, deeply integrating with the native managed services of a specific cloud platform is where much of the value of cloud can be found; for others, this cloud lead to material lock-in risks that need to be mitigated.


Notes taken from (https://www.ibm.com/cloud/learn/serverless)