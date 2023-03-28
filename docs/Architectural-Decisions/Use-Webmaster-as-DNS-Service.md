

# AD-021


### Name

Use Webmaster as DNS Service


### Status

proposed


### Last Update

2022-02-22


### Subject Area

DNS


### Topic

DNS Service Choose 


### Issue or Problem Statement

Since Cognitive Architect will move to IBM Cloud, needs to request a new domain name


### Assumptions

<br>


### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Use CIS(Cloud Internet Service) as DNS service</summary>

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
        <td>Use CIS(Cloud Internet Service) as DNS service</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><ul><li>Domain Name: Custom domain name registration</li><li>Maintenance: Controled by us, any change take effect immeditely.</li><li>Support: IBM Cloud Support Case(7*24)</li><li>SSL Certificate: privided by CIS, free. long-term expiration</li><li>Cost: 275$/month(Standard)</li><li>Onboard: None</li><li>Security: CIS provides Distributed Denial of Service (DDoS) protection, Web Application Firewall (WAF), Transport Layer Security (TLS)</li><li>Global Load balance Support: Yes<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Except DNS Capability, Could also support security &amp; Global Load balance </li><li>Domain name flexibility is better<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>Cost with 275$/month(Standard)<br></li></ul></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use Webmaster as DNS Service</summary>

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
        <td>Use Webmaster as DNS Service</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><ul><li>Domain Name: Must contains "IBM", with xxx. ibm.com or ibm.com/xxx </li><li>Maintenance: Depends on AT&amp;T and IBM team, change needs 5 business day, quarterly freeze.</li><li>Support: Slack channel, ServiceDesk(issue ticket)</li><li>SSL: one or two years expiration, more effort</li><li>Cost: None</li><li>Onboard: Complex(https://w3.ibm.com/w3publisher/corporate-webmasters)</li><li>Security: None</li><li>Global Load balance Support: No<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Domain name ends with xxx. ibm.com or ibm.com/xxx, which is good as IBM Internal Tool</li><li>No Cost<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>Can not apply to client instance. </li><li>No Security and Global Load balance Support Capability</li><li>Onboard process is complex<br></li></ul></td>
    </tr>
</table>


</details>


    



### Decision

Use Webmaster as DNS Service


### Justification

1. the inbound request is authenticated throuhg W3id Only, limits the exposure to DDoS atacks. And global loadbalance is not required capability, so CIS is not very necessary for CA internal version<br>2. The domain name ends with ibm.com is more formal for internal app<br>3. No Cost or fewer cost(Is in confirm)<br><br>


### Implications

1. Webmaster requires more onboard and maintainence effort
2. Webmaster cost is under confirm, xxx.ibm.com has no cost, ibm.com/xxx is checking the cost,  needs to discuss a new domain name



### Derived Requirements




### Related Decisions


