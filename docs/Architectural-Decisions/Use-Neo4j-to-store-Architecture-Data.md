

# AD-001


### Name

Use Neo4j to store Architecture Data


### Status

accepted


### Last Update

2017-04-01


### Subject Area

Data Storage


### Topic

Architecture Data Storage


### Issue or Problem Statement

<div>Architecture Data has very complex &amp; deep relationship, for example, there could have relationship from Logical Node -&gt; Deployment Unit - &gt; Logical Component -&gt; Physical Component, and these elements could be reused in different diagram or document. It is a challenge to store &amp; query such complex relationship.<br></div>


### Assumptions




### Motivation

Improve Architecture Data Store &amp; Query Performance<br>


### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Use Cloudant DB to store</summary>

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
        <td>Use Cloudant DB to store</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>In PoC phase, we used Cloudant to store the Architecture Data. <br></div><div>Pros: Could reuse PoC code</div><div>Cons: PoC has appeared the disadvantage to query architecture data in document database<br></div></td>
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


    

<details markdown=1>
<summary markdown="span">Use Neo4j to store Architecture Data</summary>

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
        <td>Use Neo4j to store Architecture Data</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Pros: <br></div><div>- Graph Database could store architecture data complex relationship<br></div><div>- Neo4j is the leading Graph Database, with comprehensive documents</div><div>Cons: <br></div><div>- Team has no experience on Neo4j</div><div>- Neo4j Enterprise version needs to pay<br></div></td>
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


    

<details markdown=1>
<summary markdown="span">Use OrientDB to store Architecture Data</summary>

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
        <td>Use OrientDB to store Architecture Data</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Pros:</div><div>- Could support document &amp; graph storage, document could be used for non-graph data storage</div><div>Cons:</div><div>- No much Document, and not popular as Neo4j</div><div>- More learning curve<br></div></td>
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

Use Neo4j to store Architecture Data


### Justification

<div>- To store such complex architecture data, graph database is the best choice,  and a PoC support this decision</div><div>- Neo4j is the leading graph database with much documents, it is easier to help team quickly pick up graph knowledge using neo4j</div>


### Implications

Possible to pay for Neo4j cluster along with the business increase


### Derived Requirements




### Related Decisions


