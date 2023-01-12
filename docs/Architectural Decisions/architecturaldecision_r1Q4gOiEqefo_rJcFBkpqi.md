

# AD-002

### Name

App Connect Data Layer Addition (Cloudant + COS)

### Status

accepted

### Last Update

2021-05-28

### Subject Area

Provision a dedicated Cloudant instance for App Connect usage

### Topic

App Connect data layer

### Issue or Problem Statement

Either using a dedicated or shared Cloudant instance for App Connect<div><br></div><div>    • Read/Write operations and global queries' quota limitation for the shared database instance between backend and App Connect</div><div>    • Delays resulted from waiting for R/W operations might impact App connect performance</div><div>    • A shared database would be a single point of failure for both integration and the core layer in case of outage</div><div><br></div>

### Assumptions



### Motivation

    • Solidify the integration data layer with a tenant-isolated database<div>    • Increase overall security as the App Connect layer is controlled by tenant</div><div>    • Support different availability requirements and simplify administration and backup for different backup schedules and recovery models</div><div><br></div>

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Backend and App Connect to use the same Cloudant database instance</summary>

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
        <td>Backend and App Connect to use the same Cloudant database instance</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Backend and App Connect to use the same Cloudant database instance</td>
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
<summary markdown="span">Use Dedicated Cloudant Instance</summary>

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
        <td>Use Dedicated Cloudant Instance</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Use Dedicated Cloudant Instance</td>
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

Use Dedicated Cloudant Instance

### Justification



### Implications

    • Enhancing the performance 
    • Solidifying and securing the integration data layer
    • Giving the tenant all the rights needed to control/manage App Connect database

### Derived Requirements


DevOps requirements for the backup and recovery of the new database instance

### Related Decisions



