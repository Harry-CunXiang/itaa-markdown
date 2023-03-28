

# AD-007


### Name

Use AngularJS 2 as the front-end framework


### Status

accepted


### Last Update

2017-04-20


### Subject Area

Technical stack


### Topic

Development


### Issue or Problem Statement

Instead of building afront-end framework from zero, it’s better to leverage an existing front-end framework.<br>


### Assumptions

1. The target platform is web browser, eg. desktop web browser and tablet web browser<br>2. Stable and easy to use


### Motivation

Help team to speed upthe development process


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
        <td>1. AngularJS 1.x<br>2. AngularJS 2<br>3. Backbone<br>4. React.js</td>
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

1. Written by ES6, code is more clear &amp; easy to maintain<br>2. Supports all modern web browser<br>3. Better than AngularJS 1.x (https://blog.angularjs.org/2014/03/angular-20.html?m=1)<br>4. Supports bootstrap (https://github.com/valor-software/ng2-bootstrap)<br>5. Supports external library(https://medium.com/@s_eschweiler/using-external-libraries-with-angular-2-87e06db8e5d1)


### Implications

1. Loopback does not officially supports AngularJS 2 (http://loopback.io/doc/en/lb3/AngularJS-JavaScript-SDK.html#introduction)
2. AngularJS 2 is new and lack of the resource


### Derived Requirements

N/A


### Related Decisions

N/A
