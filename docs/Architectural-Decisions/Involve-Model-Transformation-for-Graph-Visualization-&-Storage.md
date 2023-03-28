

# AD-012


### Name

Involve Model Transformation for Graph Visualization & Storage


### Status

accepted


### Last Update

2018-01-13


### Subject Area

Data Model


### Topic

Graph Visualization & Storage


### Issue or Problem Statement

1) Front-end &amp; Back-end data are coupling together now, FED needs to understand the data model in the Back-end
2) A lot of model sync in Frontend
3) Impossible to support other graph visualization tool, like D3


### Assumptions

MxGraph &amp; Neo4j has specific data schema


### Motivation

Reduce the complexity &amp; Increase extendibility


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
        <td>1） Continue current solution
2)   Involve Model Transformation</td>
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

1) Model Transformation has better extendibility and will reduce the complexity in the Frontend
2) Can support more graph Visualization in the future


### Implications

1) Need to do the data migration of history data
2) Import & Export Services have dependency here
3) Will slow down the development in current phase


### Derived Requirements




### Related Decisions


