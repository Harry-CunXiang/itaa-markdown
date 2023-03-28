

# AD-028


### Name

Backup and restore


### Status

accepted


### Last Update

2022-05-26


### Subject Area

Storage


### Topic




### Issue or Problem Statement




### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Create CA's own script to do the backup and restore manually.</summary>

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
        <td>Create CA's own script to do the backup and restore manually.</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Better to control what kind of data needs to be backup, it happens at the application level.</td>
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
<summary markdown="span">Leverage the snapshot of IBM Cloud File Storage to do the backup and restore</summary>

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
        <td>Leverage the snapshot of IBM Cloud File Storage to do the backup and restore</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>IBM Cloud File Storage service provides a snapshot feature, which supports backup, restore, etc..</td>
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

Leverage the snapshot of IBM Cloud File Storage to do the backup and restore


### Justification




### Implications




### Derived Requirements




### Related Decisions


