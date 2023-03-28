

# Risk-01 Neo4j Community Version Limitation


### Risk Description


Due to license issue, our system is using Neo4j community version now, neo4j Community Version can not support cluster.  Along with the data size increase, one single database node will probability be a bottleneck in the future. 



### BU / Department / Competency




### Owner




### Probability


Medium



### Impact


High



### Effort / Cost




### Contingency / Mitigation recommendation


<div><b>Current solutions: </b><br></div><div>1) Monitor Neo4j Status to check the database issue quickly</div><div>2) Backup Neo4j data every day.<br></div><div><br></div><div><b>Two solutions are considered in the future:</b><br></div><div>1) Switch to Neo4j Enterprise version, which will involve additional subscription cost</div><div>2) Switch to other open source graph database like Janusgraph, which could support cluster. Need a PoT to see the migration effort, performance, other consideration.<br></div>



### Date Raised




### Review Date

2018-03-01


### Date Closed




### Comments




### Is this a Key Risks?

true


### External


