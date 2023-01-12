

# AD-005

### Name

Multi-Tenant Support In Object Model

### Status

proposed

### Last Update

2021-05-28

### Subject Area

multi-tenant

### Topic

Object model multi-tenant

### Issue or Problem Statement

The object model of the product should support multi tenants

### Assumptions

The product should be generic to support multi-tenants

### Motivation

We don’t need to start from scratch when new tenant or client wants to use the product

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Create generic key value list for client specific fields and save this list along with the shipment</summary>

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
        <td>Create generic key value list for client specific fields and save this list along with the shipment</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Create generic key value list for client specific fields and save this list along with the shipment</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>ODM verbalization will not work</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Retrieve client specific fields before calling the ODM services that need these fields </summary>

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
        <td>Retrieve client specific fields before calling the ODM services that need these fields </td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Retrieve client specific fields before calling the ODM services that need these fields <div>Integration step will be added, custom code implemented everywhere</div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Integration step will be added, custom code implemented everywhere</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Standardize fields for all clients</summary>

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
        <td>Standardize fields for all clients</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Create one standardized model for the product.<div>Standardize fields for all clients and if client specific fields list expanded to be heavy, we can switch back to "Retrieve client specific fields" option</div></td>
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

Standardize fields for all clients

### Justification

    • Having a standard model will make the product more efficient and serves many clients without rework<div>    • No customized logic for each client</div>

### Implications



### Derived Requirements



### Related Decisions



