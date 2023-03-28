

# AD-022


### Name

Use BlueFringe to connect w3 network


### Status

proposed


### Last Update

2022-02-26


### Subject Area

Network


### Topic

Network Connection to w3 network


### Issue or Problem Statement

IBM Cloud clusters can not connect IBM Intranet directly


### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Blue Fringe</summary>

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
        <td>Blue Fringe</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Blue Fringe is an offering from IBM CIO Network Engineeringteam, enable connections from IBM Cloud account to IBM's Intranet: </div><div>See Link for detail introduction: https://ibm.ent.box.com/file/920198712280</div><div><br></div><div><ul><li>Intranet Service Access scope: No limitation</li><li>Maintainablity: Config firewall for new service</li><li>Cost: $500, cost of 2 Direct Link</li></ul></div><div><br></div><div><br></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Has no limitation on Intranet Service Access Scope<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>High Cost, al least $500 per month<br></li></ul></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Cirrus proxy application</summary>

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
        <td>Cirrus proxy application</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Develop a proxy application and deploy to Cirrus, which work as proxy between services in IBM Cloud and intranet servers (BluePage api).</div><div><br></div><div><ul><li>Migration workload: Develop and deploy proxy application to Cirrus.  Change endpoints in  source code </li><li>Intranet Service Access scope: No limitation</li><li>Maintainability: Effort to manage the application</li><li>Cost: Lower Initial cost, cost of Cirrus app<br></li></ul></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Relatively Lower Cost, and has no limitation on Intranet Service Access scope</li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>Needs to maintain Cirrus App<br></li></ul></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">IEB (IBM ESB Backbone)</summary>

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
        <td>IEB (IBM ESB Backbone)</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><ul><li>IEB can expose some intranet API to internet, but only BluePage API</li></ul></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>No Cost<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>Only BluePage API for now</li></ul></td>
    </tr>
</table>


</details>


    



### Decision

Blue Fringe


### Justification

BlueFringe is an offering from IBM CIO Network Engineering&nbsp;team, enable connections from IBM Cloud account to IBM's Intranet<br>- Support connect to any services in intranet


### Implications

- Cost of IBM Cloud Direct Links
- CA DevOps team need to manage network configrations and security compliance


### Derived Requirements




### Related Decisions


