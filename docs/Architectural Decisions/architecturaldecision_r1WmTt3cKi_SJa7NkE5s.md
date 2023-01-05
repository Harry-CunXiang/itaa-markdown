

# AD-001

### Name

Data Replication

### Status

proposed

### Last Update

2019-10-02

### Subject Area



### Topic



### Issue or Problem Statement



### Assumptions



### Motivation

Maintain consistent copies of data on more than one storage location to support higher availability and resiliency.<br>

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
        <td>1) Transactional Replication: addresses full initial copies of the database and then receive updates as data changes in the same order as they occur with the publisher: transactional consistency is guaranteed.<br>2) Snapshot Replication: distributes data exactly as it appears at a specific point in time; does not monitor for updates to the data. Used when data change less often.<br>3) Merge Replication: Data from two or more databases is combined into a single database. It allows both publisher and subscriber to independently make changes to the database.</td>
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

Alternative - Deprecated

### Justification

see - https://ibm-cloud-architecture.github.io/refarch-data-ai-analytics/preparation/data-replication/<br>

### Implications



### Derived Requirements



### Related Decisions



