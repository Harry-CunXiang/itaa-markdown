

# AD-015

### Name

Context data to be sent in the payload of the notification events

### Status

accepted

### Last Update

2021-08-28

### Subject Area

Sending context data in the outbound notification events

### Topic



### Issue or Problem Statement

Sending context data as a separate attribute in the notification events will add complexity in dealing with payload versioning and compression

### Assumptions



### Motivation



### Notes



[Expand all](#){ .md-button .same-line }

### Alternatives


    

<details markdown=1>
<summary markdown="span">Set context data object to the notification event payload</summary>

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
        <td>Set context data object to the notification event payload</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Any data object that is set in the context attribute (even if received from external party) and needs to be published in the notification event must be set in the payload of the event </td>
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

Set context data object to the notification event payload

### Justification



### Implications



### Derived Requirements



### Related Decisions



