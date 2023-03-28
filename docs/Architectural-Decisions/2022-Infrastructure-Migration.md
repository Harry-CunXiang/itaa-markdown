

# AD-019


### Name

2022 Infrastructure Migration


### Status

proposed


### Last Update

2022-03-21


### Subject Area

Infrastructure


### Topic

Infrastructure Migration


### Issue or Problem Statement

Bluecloud Subset by the end of 2022<br>


### Assumptions

<div>Cognitive Architect &amp; Engage! will separate the Infrastructure after the migration</div><div><br></div><div>Bluecloud suggests to move to Cirrus, and provide different architecture patterns  <a href="https://pages.github.ibm.com/CIOCloud/cio-blog/architecture-patterns/" target="_blank">https://pages.github.ibm.com/CIOCloud/cio-blog/architecture-patterns/</a>. But, Cirrus can not support Database.  </div><div><br></div>


### Motivation

<br>


### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Cirrus + CIO Private Cloud</summary>

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
        <td>Cirrus + CIO Private Cloud</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Use Cirrus to run Application Services, and use CIO Private Cloud to store data</div><div><ul><li>Cirrus to private cloud speed is  in progress improvement now</li><li>More maintenance effort<br></li></ul></div><div><br></div><div><br></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>Database resides in Intranet Network</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>There has potential performance issue between Cirrus &amp; CIO Private Cloud </td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Cirrus + IBM Cloud OCP Cluster for databases</summary>

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
        <td>Cirrus + IBM Cloud OCP Cluster for databases</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Use Cirrus run application, and use IBM Cloud OCP Cluster to manage databases</div><div><br></div><div><ul><li>Platform Consistency: </li><ul><li>Low,  our external envs are used OCP Cluster, we need to investigate Cirrus.</li></ul><li>CI/CD Migration workload:</li><ul><li> Impact:High</li><li>Complicate deveops pipeline scripts, we should change many. Microservices are controlled by Cirrus one by one, there are 4 envs * 15 = 60 microservices. We have many batch jobs,such as: batch build/batch deploy/staging blue-green/prod blue-green/databases backup/databases restore</li><li>CAES DevOps Platform can't connect to Cirrus, There are too many batch pipeline jobs, so we still need to use Jenkins to manage our jobs. We will run jenkins container in Cirrus and migrate Jenkins jobs to this;</li></ul><li>Network Connection: </li><ul><li>No connectivity issue.  Cirrus is in IBM internal network, there is no issue to connect IBM internal APIs such as Bluepage from Cirrus.</li></ul><li>Security</li><ul><li>High</li><li>Applications are deployed in W3 Network, low possibility to be attacked.</li><li>Databases are deployed in Public Network, only expose private endpoint, and support data encrypted at-rest through PV</li></ul><li>Maintainabiliy</li><ul><li>Impact: High</li><li>Need to deploy neo4j/mongo/redis in Public OCP Cluster due to persistent volume issue in Cirrue, result in maintainance in two places</li><li>Some original matianance scripts needs to do adustement to support Cirrus Env</li><li>Cirrus can not support Instana for monitor<br></li></ul><li>Support</li><ul><li>7*24 Free</li></ul></ul></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><div>- More Secured, since application deployed in W3 Network </div><div>- No Network connection issue from Internet to Intranet </div></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>- More Maintainance effort<br>- More DevOps Migration Effort<br>- Not Consistent with ITAA Environment<br>- Higher Cost</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">IBM Cloud Openshift Cluster for application services and databases </summary>

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
        <td>IBM Cloud Openshift Cluster for application services and databases </td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Run both application services &amp; databases in IBM Cloud Openshift Cluster<br><br><ul><li>Platform Consistency: <br><ul><li>Yes, same with ITAA deployment model<br></li></ul></li></ul><ul><li>CI/CD Migration workload:</li><ul><li>Impact: Low</li><li>Jenkins BlueCloud server will sunset, use CAES DevOps Platform;</li><li>We can use previous pipeline scripts which used for Multi Tenant, so little change for pipeline scripts;</li></ul><li>Connectivity issue</li><ul><li>IBM Public Cloud is in external public network, we can't directly connect IBM internal APIs such as Bluepage from Cirrus. So, need to leverage BlueFringe, Direct Link to access IBM Internal Services.<br></li></ul></ul><ul><li>Security</li><ul><li>High, but needs to be controlled more carefully</li><li>Application are deployed in Public Network, uses W3ID to make sure only IBMer &amp; OceanID can login. Only necessary port exposed.</li><li>Databases are deployed in Public Network, only expose private endpoint, and support data encrypted at-rest through PV<br></li></ul></ul><ul><li>Maintainabiliy</li><ul><li>Impact:Low</li><li>Use previous pipeline scripts to do Devops daily work, it's easier for Devops.</li></ul><li>Support</li><ul><li>7*24 Cost Included with cloud entitlements</li><li>Support on Basic Support type, not very in time<br></li></ul></ul></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td> - Platform consistency with ITAA<br>-  Less Maintainance effort<br>- Less DevOps Migration Effort<br> - Less Cost</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>- Needs to control security mare carefully as Application deployed in Public Network<br>- Internet to Intranet Connection needs to be resolved</td>
    </tr>
</table>


</details>


    



### Decision

IBM Cloud Openshift Cluster for application services and databases 


### Justification

<div>This option has less Maintenance effort, consistent with ITAA environment,  and less DevOps Migration Effort. </div><div><br></div><div>More details summary see the link </div><div><a href="https://ibm.ent.box.com/file/920548083157" target="_blank">https://ibm.ent.box.com/file/920548083157</a></div><div><a href="https://ibm.ent.box.com/file/905691161735" target="_blank">https://ibm.ent.box.com/file/905691161735</a><br></div>


### Implications

- Needs to control the external access port & permission.
- Data needs to encrypted at-rest and transmission



### Derived Requirements




### Related Decisions


