

# AD-010

### Name

Subscription And Notifications Handlers

### Status

proposed

### Last Update

2021-05-28

### Subject Area

Events subscription and notifications

### Topic

Events

### Issue or Problem Statement

To handle events subscriptions and notifications feature

### Assumptions



### Motivation



### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span"> Create a separate microservice to handle subscription & notifications</summary>

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
        <td> Create a separate microservice to handle subscription & notifications</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td> Create a separate microservice to handle subscription &amp; notifications</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Where shall we store list of events that could be subscribed to? Noting that each microservice has its own database</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Include subscription & notifications handling logic in the event handler microservice</summary>

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
        <td>Include subscription & notifications handling logic in the event handler microservice</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Include subscription &amp; notifications handling logic in the event handler microservice <div><br></div><div>    • Subscription handler component will be a part of events handler microservice</div><div>    • Notifications handler will be a new microservice</div><div>    • Notification handler will call backend API to get the payload that should be sent to the external webhook </div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Events handler will be loaded by irrelevant calls to external web hooks which may affect the performance</td>
    </tr>
</table>


</details>


    



### Decision

 Create a separate microservice to handle subscription & notifications

### Justification

    • Notifications logic that calls external system is externalized in a separate independent microservice<div>    • Events handler is not impacted</div>

### Implications



### Derived Requirements



### Related Decisions



