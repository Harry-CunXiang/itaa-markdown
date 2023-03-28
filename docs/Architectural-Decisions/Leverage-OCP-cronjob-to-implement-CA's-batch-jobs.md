

# AD-027


### Name

Leverage OCP cronjob to implement CA's batch jobs


### Status

accepted


### Last Update

2022-05-24


### Subject Area

Batch Jobs


### Topic

How to implement the batch jobs


### Issue or Problem Statement




### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Leverage OCP cronjob to implement the CA's batch jobs</summary>

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
        <td>Leverage OCP cronjob to implement the CA's batch jobs</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>1. the batch job is triggered by the OCP cronjob<div>2. create the batch job microservice, which contains the logic of batch job, including invoking backend service's API, etc..</div></td>
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
<summary markdown="span">Use CA App to trigger the batch job</summary>

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
        <td>Use CA App to trigger the batch job</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>1. CA APP triggers the batch job<div>2. the batch job's logic is placed in the individual backend service.</div></td>
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

Leverage OCP cronjob to implement the CA's batch jobs


### Justification

it's a better way to trigger and manage the job's scheduler, as well as it does not impact the release of the CA APP.


### Implications




### Derived Requirements




### Related Decisions


