

# AD-009

### Name

Post & Subscribe Events APIs Design

### Status

proposed

### Last Update

2021-05-28

### Subject Area

Events APIs design

### Topic

APIs design

### Issue or Problem Statement

Post and subscribe events APIs design in API connect

### Assumptions

All events in the system could be posted<div>A subset of these events could be subscribed to</div>

### Motivation



### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span"> Create one API to post events in general and taking event name as input</summary>

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
        <td> Create one API to post events in general and taking event name as input</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div> Create one API to post events in general and taking event name as input</div></td>
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
<summary markdown="span">Create multiple APIs to subscribe to events</summary>

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
        <td>Create multiple APIs to subscribe to events</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Create multiple APIs to subscribe to events</td>
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



### Justification

    • To have a clear catalogue of events needed in the system noting that all of these events should be accessible for post operation<div>    • For the subscription, it will be added complexity if we created separate APIs for each event in the product because not all of them will be part of the subscription.</div><div>    • The subscription handler will be responsible of maintaining the list of events that could be subscribed to</div>

### Implications



### Derived Requirements



### Related Decisions



