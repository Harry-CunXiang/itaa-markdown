

# AD-021

### Name

APIC Upgrade process

### Status

proposed

### Last Update

2022-06-07

### Subject Area



### Topic



### Issue or Problem Statement

CCS APIs are currently implemented on API Connect Sas version 5 which is sunset in April and expected end of support date is end of 2022.<div>There are two ways to perform the APIs upgrade:</div><div><ol><li>API Connect migration utility</li><li>Manual upgrade</li></ol></div>

### Assumptions



### Motivation



### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">API Connect migration utility</summary>

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
        <td>API Connect migration utility</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>There is a utility that does the upgrade from version 5 to version 10.<div>Since in AD-020 Advanced upgrade is selected --&gt; upgrade utility will need some manual effort to make the APIs compatible with version 10.</div></td>
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
<summary markdown="span">Manual uprade</summary>

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
        <td>Manual uprade</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>This approach is to manual update CCS APIs to the latest version without using any migration utility.</td>
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

Manual uprade

### Justification

<ul><li>It is risky to use upgrade utility specially that we will need to perform manual changes in all cases to support the advanced upgrade</li><li>All APIs are following the same pattern of implementation so it will not be very complicated to manual update them</li><li>Once the team is familiar with the new syntax and components of version 10, we can start implementing the APIs using the latest version and test the results</li></ul>

### Implications



### Derived Requirements



### Related Decisions



