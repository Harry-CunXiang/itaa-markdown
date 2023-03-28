

# AD-009


### Name

Define the Architecture to be composed of a collection of abstract artifacts. The system also defines a "changeable" set of concrete artifact types allowing for evolution of the scope of content documented within an Architecture.


### Status

accepted


### Last Update

2019-05-20


### Subject Area

Data Model


### Topic

How to model the documentation / artifacts associated with an Architecture


### Issue or Problem Statement

It is important that any architecture (solution, reference architecture, or architecture pattern) are constructed / documented in a consistent fashion.&nbsp; To support that a set of templates have been built to establish these standards. Tooling will present a (dynamic) TOC based on what elements are present in the specific architecture (asset). The current tool is starting small and focusing on high-valued artifacts to impact adoption and particular support those key reference architectures. However, over time, it is likely that we will want to support (at least the management of) additional artifact types. This would imply it would be best not to hardcode in the data model or the application code each of the supported artifact types but rather let that be dynamic.


### Assumptions

We don't know all of the artifact types that we will want to support during initial design time.


### Motivation

It is important to be flexible in the data model and application programming to allow the tool and repository to adapt to the evolving needs of the user community.&nbsp; Example, there is request to capture Design Thinking artifacts used to drive the architecture solution design.&nbsp; Today we focus on pre-sales, but there may be some delivery teams that might like to use the tool for pattern driven customization.


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
        <td>1. Define the Architecture to be composed of explicit artifact types, e.g., System Context, AOD Services, …<br>2. Define the Architecture to be composed of a collection of abstract artifacts. The system also defines a "changeable" set of concrete artifact types allowing for evolution of the scope of content documented within an Architecture.</td>
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

N/A


### Implications

Each concrete artifact type needs to be self-describing.  This will allow the construction of a TOC based entirely on what is present within a particular architecture asset. Implies not just the name but also tool-wide "order" so that TOCs look the same across all assets.  It means additional layers in the core meta-model.  Namely - Archtiecture has collection of Artifacts; constraint that the collection cannot have more than one instance of a particular concrete Artifact type.   That All concrete artifacts "inherit" from the Abstract artifact type and then describe their specific contents.  There will need to be code handlers for each concrete artifact type.


### Derived Requirements

N/A


### Related Decisions

N/A
