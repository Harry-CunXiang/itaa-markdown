

# AD-011


### Name

Use Neo4j Directly for Architecture & Artifact Service


### Status

accepted


### Last Update

2018-01-13


### Subject Area

Technical Stack


### Topic

Performance


### Issue or Problem Statement

1)  The sync between Mongodb &amp; Neo4j will cause the performance lost especially for Arch Copy &amp; Artifact Udpates
2) Along with more and more complex relationship in our App, Mongodb is difficult to maintain &amp; operate such complex graph relationship.




### Assumptions

1) Neo4j is stable enough
2) Neo4j Enterprise will be involved for Cluster in the future


### Motivation

Improve the System Performance


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
        <td>1) Use Neo4j for Architecture &amp; Artifact Service
2) Use Neo4j for both User , Architecture &amp; Artifact Service
3) Use other Graph DB</td>
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

1) Neo4j is the leading graph database
2) Loopback Security framework can not support Graph DB now, so, User Service will continue to use Mongodb



### Implications

1) Neo4j Doc Manager will be gave up
2) Need to make sure all the architecture & artifact data in Mongodb can sync to Neo4j
3) Need to do the data migration


### Derived Requirements




### Related Decisions


