

# AD-024

### Name

ODM multi-tenancy

### Status

proposed

### Last Update

2022-10-13

### Subject Area

ODM

### Topic

Multi-tenant

### Issue or Problem Statement

Based on the assessment of new tenants that are onboarded to Customs Compliance Platform, there are two options:<div>1. Reuse one IBM ODM on Cloud subscription to serve multiple tenants</div><div>2. Have separate IBM ODM on Cloud subscriptions for each tenant</div><div>This Architectural Decision focuses on option 1 and the alternatives of this approach</div>

### Assumptions

Assessment is done for the tenants that will be onboarded and will share the same IBM ODM on Cloud subscription. This assessment should cover several aspects such as: the shared infrastructure, expected loads...etc.

### Motivation

1. Reusing available existing resources that still have the capacity to handle extra loads for other tenants<div>2. Cost</div>

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Create new internal adaptor to act as tenants orchestrator</summary>

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
        <td>Create new internal adaptor to act as tenants orchestrator</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>A new component will be created to handle the ODM calls through pub/sub as a part of the current event-driven architecture.<div><ol><li>The feature will post event on Kafka</li><li>The adaptor will subscribe to the event and call the corresponding ODM service</li><li>ODM adaptor will parse the ODM response and post another event on Kafka for the next feature to be triggered</li><li>Failures must be handled through events</li></ol></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ol><li>Decoupling of ODM.</li><li>Including ODM to CCP event-driven architecture is more flexible an dynamic.</li><li>Extensible solution</li><li>The current approach of direct calls from the microservices and integration layers is coupling all layers together
</li></ol></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Effort needed to refactor of all backend and integration features calling ODM is needed to use the new adaptor for orchestration<br></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Event-driven using Business Automation Insights</summary>

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
        <td>Event-driven using Business Automation Insights</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Introduce Business Automation Insights to include ODM in CCP event-driven architecture. ODM will be executing the required decision services based on the posted events.</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><div><ol><li>Decoupling of ODM.</li><li>Including ODM to CCP event-driven architecture is more flexible an dynamic.</li><li>Extensible solution</li><li>The current approach of direct calls from the microservices and integration layers is coupling all layers together</li></ol></div></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>This will require to move from IBM ODM on Cloud Saas to CP4A</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Introducing routing DB2 table</summary>

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
        <td>Introducing routing DB2 table</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Introducing new DB2 table including tenant configurations. This table should support the consumers to retrieve the corresponding ODM endpoint for each feature and for each tenant.</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>Simple implementation</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ol><li>Increased DB calls to retrieve flow configuration</li><li>Having too many configured features and endpoints will make it difficult to be maintained</li><li>Possibility of errors</li></ol></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">ODM acting as tenants orchestrator</summary>

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
        <td>ODM acting as tenants orchestrator</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>ODM will be responsible for orchestrating the calls to the target tenant.<div><ol><li>Consumer will send a value representing the current tenant to the ODM decision services</li><li>ODM service will execute the rules of the input tenant</li><li>ODM will respond to the consumer with the response</li></ol></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>Simplified Backend changes. The only needed change is to pass the tenant as a parameter to all ODM decision services.</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ol><li>Very high complexity at ODM side to orchestrate and maintain all tenants flows in one ODM call</li><li>ODM is a business rules management system and should not be misused as orchestration</li></ol></td>
    </tr>
</table>


</details>


    



### Decision

ODM acting as tenants orchestrator

### Justification

<ul><li>Decoupling of applications layer. Each layer will be responsible for a clear objective:</li></ul><ol><li>ODM: Only business rules execution</li><li>Orchestrator adaptor: Orchestrate ODM calls</li><li>Micro services and integration: Execution of their main logic</li></ol><div><ul><li>Extensible solution.</li><li>Expanding Event-driven approach across all application layers</li><li>Fault tolerance and Enhanced performance through kafka</li></ul></div>

### Implications



### Derived Requirements



### Related Decisions



