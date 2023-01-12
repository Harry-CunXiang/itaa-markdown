

# AD-020

### Name

API Connect upgrade - gateway selection

### Status

proposed

### Last Update

2022-06-07

### Subject Area

API Connect

### Topic

API Connect Upgrade

### Issue or Problem Statement

CCS is currently built using API Connect Sas version 5. This version is sunset and expected end of support date to be end of 2022.<div>It is required to upgrade API Connect version to version 10.</div><div>There are two types of upgrades:</div><div>1. Simple upgrade</div><div>2. Advanced upgrade</div>

### Assumptions



### Motivation



### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Advanced upgrade</summary>

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
        <td>Advanced upgrade</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Advanced upgrade is to upgrade the APIs from version 5 to version 10 including the gateway (called native gateway)<div>Migration is not as simple as simple upgrade from implementation point of view. However, this is the latest gateway version and the performance will be significantly enhanced 5x-15x the current performance of version 5</div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>Performance is significant factor here.</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Simple upgrade</summary>

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
        <td>Simple upgrade</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Simple upgrade is easier in implementation.<div>Simple upgrade keeps using the same gateway version used by API Connect version 5.</div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>When easy and fast upgrade is needed</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>By simple upgrade:<div>performance will only be enhanced by 15%</div><div>later on, we will need to upgrade to the latest version of gateway</div></td>
    </tr>
</table>


</details>


    



### Decision

Advanced upgrade

### Justification

Advanced upgrade is the selected approach because the upgrade will be done to the latest version and also we will benefit from the performance enhancement 5-10 times the current performance of version 5.<div>It is ok to spend more time to upgrade the APIs one time to the latest and more performing version.</div><div>Also most of the APIs are implemented using the same structure so same upgrade steps will be done for all APIs. </div>

### Implications



### Derived Requirements



### Related Decisions



