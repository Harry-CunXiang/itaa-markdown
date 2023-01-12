

# AD-006

### Name

ODM Decision Services Input

### Status

proposed

### Last Update

2021-05-28

### Subject Area

ODM integration

### Topic

ODM decision services input parameters

### Issue or Problem Statement

ODM decision services input design

### Assumptions

Business users will need to update the business rules in the future based on shipment information

### Motivation

No need for IT support to update the business rules

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Discuss with business to add the candidate fields that might be used later and add them to the service input</summary>

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
        <td>Discuss with business to add the candidate fields that might be used later and add them to the service input</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Discuss with business to add the candidate fields that might be used later and add them to the service input</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>business users will only be able to change rules using these fields, there will also be many wrapper classes in ODM model and many mapping services from the caller side</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Make the input of each service only the fields that are currently required in the business rules</summary>

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
        <td>Make the input of each service only the fields that are currently required in the business rules</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Make the input of each service only the fields that are currently required in the business rules</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Business users will not be able to add new rules without referring to IT</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use shipment as the main input to all ODM services </summary>

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
        <td>Use shipment as the main input to all ODM services </td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Use shipment as the main input to all ODM services </td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>might affect performance if shipment object becomes so huge</td>
    </tr>
</table>


</details>


    



### Decision

Use shipment as the main input to all ODM services 

### Justification

    • Business users will be able to change business rules freely using any shipment field<div>    • Simplicity in ODM object model and verbalization </div>

### Implications



### Derived Requirements



### Related Decisions



