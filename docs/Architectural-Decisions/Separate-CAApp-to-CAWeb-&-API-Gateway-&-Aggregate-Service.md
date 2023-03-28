

# AD-017


### Name

Separate CAApp to CAWeb & API Gateway & Aggregate Service


### Status

accepted


### Last Update

2020-03-09


### Subject Area

Service Interaction


### Topic

Microservice Evolve


### Issue or Problem Statement

<div>Currently, CAApp is becoming more and more complex. It handles too many things like below</div><div>1. Service Aggregate</div><div>2. API Security Control(Authentication &amp; Authorization)</div><div>3. Scheduler</div><div>4. Error Handler</div><div>5. API Navigation (Manual Route )</div><div><br></div><div>And potentially will add API Rate Limit and refine API route through config.<br></div><div><br></div><div>It takes too many responsibilities and contains many configurations, making this service become more and more complex and difficult to maintain.</div><div><br></div><div>Besides, as the API Gateway &amp; Aggregate logic are mixed together in one service, it will be difficult to scale separately in the future if needed. <br></div><div><br></div><div>Also, the current deployment model, the CAWeb is a deployment unit of CAAPP, which makes the maintenance even more complex. Even small changes on the CAWeb, it's required to build and deploy the whole CAAPP.</div><br><div><br></div><div><br></div><br>


### Assumptions

<div>- The change has no influence on Front-End Integration</div><div>- The service separation could be handled with limit code influence in Back-End</div><div>- Do not involve heavy middleware<br></div><div><br></div>


### Motivation

Evolve Microservice Architecture &amp; reduce the component complex


### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Separate CAApp to API Gateway & Aggregate Service, and use API Connect as API Gateway</summary>

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
        <td>Separate CAApp to API Gateway & Aggregate Service, and use API Connect as API Gateway</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>One is for Service Aggregate, another is for API Gateway responsibilities like Secure API, Route API, API Rate Limit, etc. <br><div>And involve API Connect as API Gateway</div><div>Pros:</div><div>- Comprehensive capabilities</div><div>- Managed by Cloud, easy to do cluster</div><div><br></div><div>Cons:</div><div>- Need pay for it</div><div>- Heavy, need investigate how to integrate with current Node.js Framework<br></div></td>
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
<summary markdown="span">Separate CAApp to API Gateway & Aggregate Service, and use Express Gateway as API Gateway</summary>

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
        <td>Separate CAApp to API Gateway & Aggregate Service, and use Express Gateway as API Gateway</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>One is for Service Aggregate, another is for API Gateway responsibilities like Secure API, Route API, API Rate Limit, etc. <div>And involve Node.js Open source - Express Gateway(https://github.com/ExpressGateway/express-gateway) as API Gateway implementation to reduce code changes</div><div><br></div><div>Pros: <br></div><div> - Express Gateway is light</div><div> - Based on Node.js<br></div><div> - Do not involve new middleware</div><div>Cons:</div><div>-  No OpenID Integration</div><div>-  No User Interface<br></div><div>- Socket <br></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>N/A<br></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>N/A<br></td>
    </tr>
</table>


</details>


    



### Decision

Separate CAApp to API Gateway & Aggregate Service, and use Express Gateway as API Gateway


### Justification

 - Reduce the component complexity &amp; coupling, make it easier to maintain <br><div> - Can scale API Gateway &amp; Aggregate Service separately</div><div> - Express Gateway could meet current requirement with least impact<br></div><div> - Follow Microservice Best Practice(https://microservices.io/patterns/apigateway.html)</div><div><br></div>


### Implications

- Need to change some back-end code logic, like ACL control
- Increased deployment complexity - the API gateway is yet another moving part that must be developed, deployed and managed
- Increased response time due to the additional network hop through the API gateway - however, for most applications the cost of an extra roundtrip is insignificant.


### Derived Requirements

N/A


### Related Decisions

N/A
