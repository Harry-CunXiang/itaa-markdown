

# AD-026

### Name

Cloud Foundry Alternative For CCP Frontend

### Status

proposed

### Last Update

2023-01-10

### Subject Area

Cloud Platform

### Topic

Deprecation of IBM Cloud Foundry

### Issue or Problem Statement

IBM Cloud Foundry&nbsp;Service is planned to be sunset by June 1, 2023. Another service or component is needed to host CCP Frontend web application.<div><br></div><div>There are three options available to host CCP Web Application:</div><div><ol><li>IBM Cloud Code Engine</li><li>IBM Cloud Kubernetes Service</li><li>Red Hat OpenShift on IBM Cloud
</li></ol></div><div>An assessment is required to compare the different alternatives from different aspects such as elasticity, cost, maintainability</div>

### Assumptions



### Motivation



### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">IBM Cloud Code Engine</summary>

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
        <td>IBM Cloud Code Engine</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>IBM Cloud Code Engine is a fully managed, serverless platform that runs your containerized workloads<div><br></div><div>Ref. https://cloud.ibm.com/docs/codeengine</div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><div><div><b>Elasticity: </b>Auto-scaling based on number of HTTP requests is built in (Minimum instances are down to zero and max instances are up to 250 instance)<br></div><div><b>Cost: </b>Only pay for when workloads run (GB-sec, vCPU-sec &amp; invocations)</div><div><b>Management:</b> Managed Application. No container, cluster, networking, or infrastructure skills required</div><div><b>Monitoring:</b> Will be monitored using New Relic</div><div><b>DevOps:</b> Integrated with IBM Cloud Pipelines</div></div></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">IBM Cloud Kubernetes Service</summary>

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
        <td>IBM Cloud Kubernetes Service</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>IBM Kubernetes container orchestration&nbsp;platform.<div><br></div><div>Ref. https://cloud.ibm.com/docs/containers</div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>
<div><b>Elasticity: </b>Auto-scaling based on number of HTTP requests is built in.
</div><div><b>Management:</b> Managed Cluster<br></div><div><b>Monitoring:</b> Will be monitored using New Relic
</div><div><b>DevOps:</b> Integrated with IBM Cloud Pipelines</div></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><div><b>Cost: </b>Cluster (size of cluster * time) + integrations (GB-time) + load balancers (cost * time)</div></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Red Hat OpenShift on IBM Cloud</summary>

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
        <td>Red Hat OpenShift on IBM Cloud</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>A managed Red Hat OpenShift cloud service that reduces operational complexity and helps organizations build and scale applications with the security of IBM Cloud<div><br></div><div>https://www.ibm.com/eg-en/cloud/openshift<br><div>
</div></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><div><b>Elasticity:</b> On Red Hat OpenShift on IBM Cloud, applications are synonymous to pods. With Kubernetes, you can automatically scale up or down your pods based on CPU or memory</div><div><b>Management:</b> Managed Cluster<br></div><div><b>Monitoring: </b>Will be monitored using New Relic</div><div><b>DevOps: </b>Integrated with IBM Cloud Pipelines</div></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><b>Cost:</b> OCP license + Cluster (size of cluster * time) + integrations (GB-time) + load balancers (cost * time) Can obtain an OCP license if you get Cloud Paks</td>
    </tr>
</table>


</details>


    



### Decision

IBM Cloud Code Engine

### Justification

Minimal migration effort
<div><br></div>

### Implications



### Derived Requirements



### Related Decisions



