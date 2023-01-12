

# AD-003

### Name

App Connect Kafka vs. MQ Support For Logging Optimization (Kafka Standard) - Compare With MQ In The Cloud Pak

### Status

accepted

### Last Update

2021-05-28

### Subject Area

Event streaming vs. Messaging for App connect logger

### Topic

App Connect Logging

### Issue or Problem Statement

    • The current logging service (LogDNA) truncates large payload, so a customized logger application is developed to store payloads in cloud object storage while using LogDNA Ingest API to log COS URLs<div>    • LogDNA Ingest API is having a performance impact on application performance because of the consumed time for logging</div>

### Assumptions

Usage of common services for logging and monitoring provided by IBM Cloud Paks for Integration might eliminate the need for a customized logger application.

### Motivation

Introducing a messaging layer that would consume logging events without impacting application performance with the time consumed for logging, it’s recommended to use Kafka for that purpose.<div><br></div><div>The advantages of Kafka over MQ messaging is as follows:</div><div>    • Message Persistence</div><div>    • Topic partitioning</div><div>    • Message sequencing</div><div>    • Load balancing</div><div>    • Automatic failover &amp; High availability</div><div><br></div><div><br></div>

### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Event Streaming For Logging</summary>

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
        <td>Event Streaming For Logging</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Event Streaming For Logging</td>
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
<summary markdown="span">IBM MQ provided by IBM cloud Pak for Integration</summary>

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
        <td>IBM MQ provided by IBM cloud Pak for Integration</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>IBM MQ provided by IBM cloud Pak for Integration</td>
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

Event Streaming For Logging

### Justification

Kafka will support real time processing which is necessary for logging accuracy<div>The logger component requires a messaging system that has high retention and persistence also a very accurate real time processing so for that:</div><div><br></div><div>Kafka event streaming retains the messages even after all the subscribers have read the message and the retention period is a configurable parameter, this makes Kafka more reliable than MQ cause of message retention and state management based on the consumer offset.</div><div><br></div>

### Implications

    • A more reliable logging mechanism, with no impact on business applications
    • Isolating the logger component with its consumption (CPU/Memory)
    • Logging time is not consumed from message processing time


### Derived Requirements



### Related Decisions



