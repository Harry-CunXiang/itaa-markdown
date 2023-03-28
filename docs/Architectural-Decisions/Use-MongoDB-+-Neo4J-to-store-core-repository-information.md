

# AD-002


### Name

Use MongoDB + Neo4J to store core repository information


### Status

accepted


### Last Update

2017-03-20


### Subject Area

Database Selection


### Topic

Core Repository build up


### Issue or Problem Statement

Because the architecture contain many relationship, the query performance will be worse while the query depth is more than 3 in relational database or document database, so it is necessary to select a polyglot persistence solution<br>


### Assumptions

N/A<br>


### Motivation

1. Graph database is good at querying data relationships, which is a weakness of other NoSQL and SQL solutions. But the the performance of query will decrease while put much properties in the node or link<br>2. NoSQL database is good at store unstructured documents and good at single CRUD operations. It will be good to take each advantage of Graph database &amp; NoSQL database and use together.<br>3. After we have two different database, we need to build up the synchronization mechanism between Graph database &amp; NoSQL database to make data consistence


### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Alternative - Deprecated</summary>

<table>
    <caption></caption>
    <thead>
        <tr>
            <th></th>
            <th></th>
        </tr>
    </thead>
    <tr>
        <td> <strong>Name</strong> </td>
        <td>Alternative - Deprecated</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>1. Cloudant&nbsp; + Neo4J<br><blockquote>Pros: 1) BlueMix provides service, easier to setup/scale database environment &amp; replication<br>Cons: 1) Dedicated Bluemix needs paid 2) No ready-made communication mechanism between Cloudant with Neo4J, needs to build from scratch 3) Cloudant does not provides transaction, could not ensure data consistency in application layer<br></blockquote>2. MongoDB + Neo4J<br><blockquote>Pros: 1) Neo4J provides neo4j doc manager which can real-time migrate mongodb contents/relationship to Neo4J.&nbsp; The neo4j doc manager brief introduction could be referenced here https://neo4j.com/developer/mongodb/#_neo4j_doc_manager<br>Cons: 1) Needs to setup MongoDB environment &amp; scale locally&nbsp; 2) MongoDB does not provides transaction, could not ensure data consistency in application layer<br></blockquote><div>3. OrientDB</div><blockquote><div>Pros: 1) Can support both graph &amp; document natively, means that do not need to combine two databases, one database can cover both<br></div><div>Cons: 1) Use case &amp; documents are not as much as Neo4J</div></blockquote><div>4. DB2 + Neo4J<br></div><blockquote><div>Pros: 1) Both DB2 &amp; Neo4J support transaction, so can use XA Transaction to support distribution transaction in application layer<br>Cons: 1) The application layer will be a more complex 2) Can not support unstructured document<br></div></blockquote></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    



### Decision




### Justification

1. Neo4J is relatively the most mature graph database with highest market occupancy and comprehensive documents, and provides some integration with other database.<br>2. Neo4J provides neo4j doc manager which provides a real-time synchronization between MongoDB + Neo4J in background, but not provides synchronization for Cloudant<br>3. Enable data consistency in database level will be easier for future development and maintainment<br>Justification


### Implications

1. Neo4j community license is under GPL v3.0 and do not support scalable, needs to decide use community or use enterprise with paid. Community & Enterprise comparison link as below https://neo4j.com/editions/
2. Needs to determine which architecture contents & relationship need to be migrated to neo4j


### Derived Requirements

N/A


### Related Decisions

AD-011
