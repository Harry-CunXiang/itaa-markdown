

# AD-004

### Name

Multi-Tenant Support In ODM Decision Services

### Status

superseded

### Last Update

2021-05-28

### Subject Area

multi-tenant

### Topic

ODM decision services multi-tenant

### Issue or Problem Statement

ODM decision services should support multi tenants

### Assumptions

Many business rules are applicable for different tenants and clients

### Motivation

We don’t need to start from scratch when new tenant or client ask for the same business rules.

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Create separate BOM projects per tenant based on the common XOM project</summary>

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
        <td>Create separate BOM projects per tenant based on the common XOM project</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>    • Each tenant will have its own decision service<div>    • Tenant handling logic will be the responsibility of the caller to call the decision service of this tenant</div></td>
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
<summary markdown="span">Create separate XOM & BOM for each tenant</summary>

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
        <td>Create separate XOM & BOM for each tenant</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Create separate XOM &amp; BOM for each tenant</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Too complex given that XOM is somehow generic and standard</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Embed the tenant handling logic in the decision service</summary>

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
        <td>Embed the tenant handling logic in the decision service</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Embed the tenant handling logic in the decision service</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Means that one decision service will serve multiple tenants – complex security handling and deployment issues</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use the same BOM for all tenants</summary>

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
        <td>Use the same BOM for all tenants</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Use the same BOM for all tenants </td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>That will cause lookups privacy issue and availability of client specific fields in the verbalization</td>
    </tr>
</table>


</details>


    



### Decision

Create separate BOM projects per tenant based on the common XOM project

### Justification

    • Client specific lookups will not be accessible by all clients when BOM is different<div>    • No dependency for deployment of decision services in any tenant</div><div>    • Simple ODM decision services governance and security</div>

### Implications



### Derived Requirements



### Related Decisions

Superseded by AD-024

