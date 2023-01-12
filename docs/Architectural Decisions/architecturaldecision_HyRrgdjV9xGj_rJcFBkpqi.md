

# AD-011

### Name

Post Events APIs Design

### Status

proposed

### Last Update

2021-05-28

### Subject Area

Post event API design

### Topic

APIs design

### Issue or Problem Statement

The client needs to have the option to post an object (shipment, consignment... etc) and event in one call.

### Assumptions



### Motivation



### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Create separate APIs in API connect, one to post event and the other to post object and event</summary>

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
        <td>Create separate APIs in API connect, one to post event and the other to post object and event</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Create separate APIs in API connect, one to post event and the other to post object and event</td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Code Duplication</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Filing handler will handle this logic and API connect will only call one URL</summary>

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
        <td>Filing handler will handle this logic and API connect will only call one URL</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>    • Filing handler will handle this logic and API connect will only call one URL. To simplify error handling as it became scattered between two layers leading to complexity<div>    • Filing handler and event handler may be merged later as event handler doesn’t do anything without filing handler</div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>This alternative is simple to implement and maintain</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Handle this logic in APP connect</summary>

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
        <td>Handle this logic in APP connect</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Handle this logic in APP connect</td>
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
<summary markdown="span">One API will be created for each event</summary>

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
        <td>One API will be created for each event</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>    • One API will be created for each event<div>    • Payload parameter will be optional</div><div>    • If payload is provided, post object then capture event (business id will be provided twice – in payload and event)</div><div>    • If payload is not provided, just capture event</div><div><br></div><div>If payload is sent to the API, post object and then post event. Otherwise, only event will be posted.</div></td>
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

Filing handler will handle this logic and API connect will only call one URL

### Justification

Simplicity - one API for each event and the caller should decide whether he wants to send payload or not

### Implications



### Derived Requirements



### Related Decisions



