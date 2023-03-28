

# AD-025


### Name

Use Classic OCP Cluster


### Status

proposed


### Last Update

2022-02-26


### Subject Area

Infrastructure


### Topic

OCP Cluster Choose


### Issue or Problem Statement

It needs to request a OCP  cluster on IBM Cloud to host our app. There are two type of the cluster: Classic and VPC. We need to decide which cluster type should be used for now.


### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Classic</summary>

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
        <td>Classic</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Clusters on classic infrastructure include all the Red Hat OpenShift on IBM Cloud mature and robust features for compute, networking, and storage.</div><div><ul><li>Security: Classic clusters have many built-in security features that help you protect your cluster infrastructure, isolate resources, and ensure security compliance. </li><li>High availability: the master includes three replicas for high availability. </li><li>Cluster Network: Communication to the cluster master can be on the public or private cloud service endpoint.</li><li>App Network: All pods are routed between worker nodes on the worker node private IP address of the private VLAN. To expose the app on the public network, your cluster must have worker nodes on the public VLAN. Then, you can create a NodePort, LoadBalancer (NLB), or Ingress (ALB) service.</li><li>Storage: Can choose from non-persistent and persistent storage solutions such as file, block, object, and software-defined storage.<br>We use file stroage in our extenal envs, file stroage is suitable for:<br>- Mix of structured and unstructured data<br>- Shared data with many users at once</li></ul></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Can support File Storage<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">VPC</summary>

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
        <td>VPC</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>With VPC, you can create your cluster in the next generation of the IBM Cloud platform, in your Virtual Private Cloud. VPC gives you the security of a private cloud environment with the dynamic scalability of a public cloud, with the ability to deploy your cluster worker nodes as generation 2 compute virtual servers. </div><div><ul><li>Security: With VPC, your cluster runs in an isolated environment in the public cloud. Network access control lists protect the subnets that provide the floating IPs for your worker nodes.</li><li>High availability:  the master includes three replicas for high availability. </li><li>Cluster networking: Unlike classic infrastructure, the worker nodes of your VPC cluster are attached to VPC subnets and assigned private IP addresses. The worker nodes are not connected to the public network, which instead is accessed through a public gateway, floating IP, or VPN gateway.</li><li>App networking: All pods are routed between worker nodes on the worker node private IP address of the private VPC subnet. To expose the app on the public network, you can create a Kubernetes LoadBalancer service, which provisions a VPC load balancer and public hostname address for your worker nodes.</li><li>Storage: For persistent storage, use block, but block storage is best suited for static files that aren’t changed often because any change made to a file results in the creation of a new object.<br></li></ul></div></td>
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

Classic


### Justification

 - Platform Consistency, Multi Tenant use Classic Cluster now;<br> - VPC cluster only provided VPC Block Storage, but Block Storage is best suited for static files that aren’t changed often because any change made to a file results in the creation of a new object. So we will get low performance if we use VPC Block Storages; 


### Implications




### Derived Requirements




### Related Decisions


