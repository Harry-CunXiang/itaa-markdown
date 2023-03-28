

# AD-004


### Name

Core Repository use Excel format to load data


### Status

accepted


### Last Update

2017-03-20


### Subject Area

Data prepare


### Topic

Core Repository build up


### Issue or Problem Statement

We have to support different format documents in the future, even ppt, svg, etc... But it is difficult to parse and load the different format documents to core repository directly


### Assumptions

Provides Standard for Excel file<br>


### Motivation

Needs to provides an easy and common way to load data from document to core repository


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
        <td>1. Use Excel asstandard document<br>2. Use JSON as standard document<br>3. Use CSV as standard document</td>
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

1. Needs to provide a way to help user construct the architecture through csv directly, JSON is a little difficult to do it. CSV and Excel are relatively easier to do it.<br>2. Excel can have multiple sheets in one file


### Implications

N/A


### Derived Requirements

N/A


### Related Decisions

AD-001
