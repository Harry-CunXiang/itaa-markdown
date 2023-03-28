

# System Scalablity


### ID

NFR-03


### Name

System Scalablity


### Description

Easier to scale along with data size & network request increase.
Leverage IBM Cloud, provides 4 worker nodes to support application request. Monitor the node health, and have the capability to add new worker node if need.
From data perspective, Neo4j community version cannot support cluster, potentially to migrate to other graphdb supporting cluster while the data size increase much in the future. Will record this as a risk.


### Theme


Scalability



### Context




### Value




### Growth Rate




### Acceptance Criteria


- Could monitor current Server capability(cluster, pod, service), including cpu, memory, disk size
- In ICP/Kubernetes Cluster, could add new worker node, or increase existed worker node capability along with the business growth



### Priority


Critical



### Source




### Reference




### Test Method


Performance test



### Owner




### Review Date

2022-05-19
