

# AD-022

### Name

API Connect upgrade environment selection

### Status

accepted

### Last Update

2022-12-27

### Subject Area

Infrastructure

### Topic

Selection of an alternative for API-Connect.

### Issue or Problem Statement

CCS APIs are currently implemented on API Connect SasS version 5 which is expected to sunset by end of Jul 2023. The cloud team informed of few options that we can choose from going forward.<div><br><div>There are three options to host APIs using version 10:</div><div><ol><li>Cloudpak for integration: on openshift anywhere
</li><li>IBM API Connect: Deployable on-prem or any cloud, bring your own openshift or K8 or Ovas on VMware</li><li>IBM Cloud: Reserved instance is a managed single tenant instance with ability to add on-prem gateways</li></ol></div><div>Assessment is needed to compare the three approaches from different perspectives such as cost, maintainability, management, DR and support</div></div>

### Assumptions

<div><br></div>Cloud Pak for Integration is already used in the solution to utilize App-Connect.

### Motivation

Achieve best performance and control with minimum cloud and services cost.

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">AWS API-Connect SaaS</summary>

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
        <td>AWS API-Connect SaaS</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>A shared API-Connect SaaS model is provided on AWS.<div><br></div><div>References: https://aws.amazon.com/marketplace/pp/prodview-b3u5z3pv4wccg</div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li><b>Management: </b>Operation support will be the responsibility of the AWS Team.</li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li><b>Cost: </b>$9000 for 50M API calls with a commitment for 12 months.</li><li><b>Performance: </b>Slower performance due to hosting on two different cloud providers.<b>
</b></li><li><b>Network Traffic:</b> Network delays and network cost will be expected since the rest of the Environment is hosted on IBM Cloud while the API-C will be hosted on AWS.</li><li><b>Management:</b> the operation team has to deal with two different management layers.</li><li><b>Monitoring:</b> Separate monitoring will be needed and also need to be correlated with the rest of the environment hosted on IBM Cloud.</li><li><b>DevOps Integration:</b> Will require two different set of DevOps management. One for AWS API-C services and another one for IBM Cloud Services.</li></ul></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use API-Connect as part of the Cloud Pack for Integration</summary>

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
        <td>Use API-Connect as part of the Cloud Pack for Integration</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Leverage the current usage of the Cloud Pak for Integration (CP4I) to serve API-Connect as well as App-Connect functionalities.</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><div><ul><li>Utilize existing knowledge and support of the CP4I<br></li><li><b>Monitoring: </b>Will utilize the monitoring system used for the other components hosted on the IBM Cloud (e.g. New Relic)
</li><li><b>
Network Traffic: </b>Utilizing the IBM Cloud internal free traffic between the components.
</li><li><b>DevOps Integration:</b> Will use the IBM Cloud Pipelines <br></li></ul></div><div><br></div></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li><b>Cost: </b>Requires extra licenses for API-Connect by extending the current licenses used for App-Connect as part of the CP4I.<br></li><li><b>Performance: </b>More control over performance since the infrastructure is managed by the team.</li><li><b>Management:</b> Extra operation effort will be expected from the support team to support the new API-Connect on CP4I<br></li></ul><div></div><div><b><br></b></div></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use a Cloud Dedicated API-Connect Instance</summary>

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
        <td>Use a Cloud Dedicated API-Connect Instance</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>A new service for API-Connect using a dedicated instance will be provided by the IBM cloud. This dedicated instance will be managed by the IBM cloud team.</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Operation support will be the responsibility of the IBM Cloud Team.</li><li><b>Network Traffic:  </b>Utilizing the IBM Cloud internal free traffic between the components.</li><li><b>Management: </b>Management will be done by the SaaS provider team.</li><li><b>Monitoring: </b>Will be monitored a service response time only since it is a SaaS service.</li><li><b>DevOps Integration: </b>Will use the IBM Cloud Pipelines </li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li><b>Cost: </b>Dedicated Instance is usually higher cost than a shared SaaS or self operated models.
</li><li><b>Performance: </b>Performance could be impacted by noisy neighbors since it is a SaaS service.</li></ul></td>
    </tr>
</table>


</details>


    



### Decision

Use API-Connect as part of the Cloud Pack for Integration

### Justification

Minimize the cost and leverage the existing Cloud Pak for Integration installation and support.

### Implications

Extra effort and license will be required.

### Derived Requirements



### Related Decisions



