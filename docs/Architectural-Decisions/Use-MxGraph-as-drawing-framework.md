

# AD-006


### Name

Use MxGraph as drawing framework


### Status

accepted


### Last Update

2017-03-20


### Subject Area

Technical stack


### Topic

Development


### Issue or Problem Statement

Instead of building fromscratch, it’s better to reuse an existing drawing framework to render the architecture diagram in the browser.<br>


### Assumptions

1. Considering the browser first and keep in mind that we may need it work in mobile devices.<br>2. Offline support is necessary<br>3. Multiple User Collaboration support will be useful for us in the long term


### Motivation

Help user to draw the architecture diagram through browser


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
        <td>We did a comprehensive comparison between different browser drawing library from different perspectives, and summary 3 alternatives: Rappid, JointJS, MxGraph.</td>
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

1. MxGraph can support complex drawing elements and easy to do customization, besides of that, MxGraph also provides us the base framework of palette, properties windows, menu.<br>2. MxGraph supports mobile browser with enhanced events/user experience<br>3. MxGraph support offline edit and save<br>4. MxGraph is open source


### Implications

1. MxGraph does not support multiple user collaboration, needs to develop from scratch on it in the future.
2. MxGraph UI is not attractive, needs to customize the UI theme


### Derived Requirements

N/A


### Related Decisions

N/A
