

# AD-016


### Name

Which type of Cluster in IBM Cloud will be used for External Client?


### Status

accepted


### Last Update

2019-01-23


### Subject Area

Infrasturcture


### Topic

Which type of Cluster in IBM Cloud will be used for External Client?


### Issue or Problem Statement

It needs to request a Kubernetes cluster on IBM Cloud to host our app. There is two type of the cluster. We need to decide which should be used for now.


### Assumptions

N/A


### Motivation




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
        <td><ol><li>Public Cluster<br></li><ul><li>Public VLAN - $15</li><li>Private VLAN - $15</li><li>Simple Configuration</li><li>Accessible by public net</li></ul><li>Private Cluster</li><ul><li>You have specific security requirements or need to create custom network policies and routing rules to provide dedicated network security.</li><li>This can improve security by blocking unwanted outbound/inbound access to nodes.</li><li>Removing IP addresses means external services won't be accessible from the nodes</li><li>Gateway Appliance - $411.66</li><li>Complicated Configuration</li><li>More Security</li><li>Only Accessible by private VLAN</li></ul></ol></td>
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

<ol><li>Due to the cost limitation. We can also choose the private cluster for future deployment and the cost can be covered by client.</li><li>We have Internet service to cover the security requirements.</li><li>We also have Access Control supported by APP ID.</li></ol>


### Implications




### Derived Requirements




### Related Decisions


