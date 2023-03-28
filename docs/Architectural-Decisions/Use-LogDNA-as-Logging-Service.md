

# AD-024


### Name

Use LogDNA as Logging Service


### Status

proposed


### Last Update

2022-02-26


### Subject Area

Logging


### Topic

Logging Tool Choose


### Issue or Problem Statement

Need to keep application log history to monitor and debug issues


### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Use ELK Stack</summary>

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
        <td>Use ELK Stack</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Use ELK stack to store logs, including Kibana, Filebeat, etc</div><div><ul><li>Migration workload: Deploy and config ELK/Kibana/Filebeat containers </li><li>Maintainability: Need to manage ELK resources, patching  etc.</li><li>Support: No</li><li>Cost: Use cluster resources<br></li></ul></div><div><br></div><div><br></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Log Data maintained within cluster, easy to control the duration</li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>High Maintainability Effort<br></li></ul></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use LogDNA</summary>

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
        <td>Use LogDNA</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div><ul><li>Migration workload: Easy,  config LogDNA for OpenShift cluster</li><li>Maintainability: No effort needed</li><li>Support: IBM Cloud</li><li>Cost: 7 days $1/ GB Month, 14 days $2,  30 days $3.<br></li></ul></div><div><br></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>No Maintenance Effort<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    



### Decision

Use LogDNA


### Justification

1. No Deploymen &amp;  Maintain Effort<br>2. Easy to use


### Implications

'1. 'LogDNA includes additional cost. And cost increases aloing with the log data. Need evaluate the cost


### Derived Requirements




### Related Decisions


