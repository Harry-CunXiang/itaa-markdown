

# AD-005


### Name

Use Loopback as API framework


### Status

accepted


### Last Update

2019-05-20


### Subject Area

Technical stack


### Topic

Development


### Issue or Problem Statement

Instead of building an APIframework, it’s better to reuse an existing one.<br>


### Assumptions

N/A<br>


### Motivation

Help team to speed up the development progress.<br>


### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Alternative - Deprecated</summary>

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
        <td>Alternative - Deprecated</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>There are lots of otherframeworks, such as Express, Hapi, Sails, Restify, Meteor and so on. Here is the comparison among those frameworks. http://loopback.io/resources/#compare</td>
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

1. Loopback supports multiple database<br>2. Loopback supports to generate API from the defined data model<br>3. Loopback does not only provides sever side capability, but also provides the client side SDK.<br>4. Loopback is highly-extensible, well documented and open source<br>5. Loopback is supported by IBM/StrongLoop


### Implications

API is based on Node.js


### Derived Requirements

N/A


### Related Decisions

N/A
