

# AD-026


### Name

Use IBM SMTP server as Email Service


### Status

proposed


### Last Update

2022-02-26


### Subject Area

Notification


### Topic

Email Service


### Issue or Problem Statement

CA needs SMTP server to send mail to users


### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">SendGrid</summary>

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
        <td>SendGrid</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><div>Email Service provided by IBM Cloud</div><div><ul><li>Migration workload: Easy, change configuration</li><li>Cost: $15/month, 100,000 email</li><li>Not depend on IBM Intranet connection<br></li></ul></div></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>Not depend on IBM Intranet connection<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>Has cost<br></li></ul></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use IBM Internal SMTP Server</summary>

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
        <td>Use IBM Internal SMTP Server</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><ul><li>Migration workload: No</li><li>Cost: No</li><li>Dependency: Depend on connection to W3 Network<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><ul><li>No Cost<br></li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>Needs to connect to W3 Network<br></li></ul></td>
    </tr>
</table>


</details>


    



### Decision

Use IBM Internal SMTP Server


### Justification

<ul><li>No Cost</li><li>with BlueFringe, CA can connect to IBM Intranet</li></ul>


### Implications




### Derived Requirements




### Related Decisions


