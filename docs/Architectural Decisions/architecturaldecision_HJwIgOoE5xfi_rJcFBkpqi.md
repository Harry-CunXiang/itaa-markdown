

# AD-014

### Name

DB2 High Availability

### Status

proposed

### Last Update

2021-07-11

### Subject Area



### Topic



### Issue or Problem Statement

DB2 currently is not highly available, it implements DR solution with manual failover to the DR node.<div>Since we host our Tenant handler and Masterdata handler components on DB2, any outage will cause the full CCS system to be unreachable.</div><div><br></div><div>One of the questions that needs to be answered is: do we need high availability for both tenanthandler and master data handler? or only tenant handler (since master data handler can be a recoverable)</div><div><br></div>

### Assumptions



### Motivation

Keep the system up and running even after failure of DB2

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Find an alternative database component and keep replicating to it in the background (may be a manual replication)</summary>

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
        <td>Find an alternative database component and keep replicating to it in the background (may be a manual replication)</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Find an alternative database component and keep replicating to it in the background (may be a manual replication)</td>
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
<summary markdown="span">Keep using the DR-HA option of DB2</summary>

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
        <td>Keep using the DR-HA option of DB2</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Keep using the DR-HA option of DB2 and accept an amout of system outage according to Nike RPO &amp; RTO requirements.</td>
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



### Implications



### Derived Requirements



### Related Decisions



