

# AD-016

### Name

Implement Pub-Sub Pattern

### Status

proposed

### Last Update

2021-09-13

### Subject Area



### Topic



### Issue or Problem Statement

1) Every event will have a dedicated topic where it will be published<div>2) Microservices will be subscribed to the event topic of interest</div><div>3) Process rules can no longer be changed without downtime so a new design has to be set to replace the process rules concept</div><div>4) A single consumer in a microservice (as the notification service) can listen to multiple event topics</div><div>5) Backlog for a single consumer to multiple topics can be eliminated by horizontal scaling</div><div>6) Each microservice can have multiple consumer groups to serve multiple purposes</div><div>7) ELK can subscriber to the event topics directly without the notification service involved? The goal is to treat ELK as an external system and receive events only from notification microservice.</div><div>8) The number of topics might explode due to the number of events</div><div>9) Events for the same purpose such as missing, retry and failed for the same feature can be emitted on the same topic</div><div>10) Implementing the pub/sub should involve a load redistribution which will result in performance boost.</div><div>11) Notification microservice will start receiving events in a more real-time approach (example: it will not depend on event handler to produce a new event, …)</div>

### Assumptions



### Motivation

Improve the system's performance, better handling of the system resources, more control on scalability.

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Implement Pub-Sub</summary>

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
        <td>Implement Pub-Sub</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Implementation of pub-sub pattern that requires the message to be produced only once and consumed by several subscribers</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>When fast processing is needed.<div>No polling is required since message topics allow instantaneous, push-based delivery.</div><div>Independent decoupling and scaling - each subscriber will determine its own scale and pace of processing messages.</div></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Careful design and maintaining a stable contract is needed to avoid making the pub-sub communication error-prone.</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Keep Using Message Queue</summary>

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
        <td>Keep Using Message Queue</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Current implementation is more into a Message Queue at which the publisher knows exactly the subscribers interested in a specific topic. </td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>When it is important that each message is processed (and only processed once), but it is not necessary to process messages in order.</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Constraints on scalability and having multiple consumers process the same message. Usually needs the message to be produced multiple times to notify all consumers.<div>Some topics are causing bottlenecks (to be produced and consumed) and their messages could be processed in parallel (e.g., monitoring topics)</div></td>
    </tr>
</table>


</details>


    



### Decision

Implement Pub-Sub

### Justification

Improve the system's performance, better handling of the system resources, more control on scalability.

### Implications



### Derived Requirements



### Related Decisions



