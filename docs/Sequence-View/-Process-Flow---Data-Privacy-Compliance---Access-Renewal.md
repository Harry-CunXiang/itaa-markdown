

## Diagram

![ Process Flow - Data Privacy Compliance - Access Renewal](../img/cmdynamicview_Bku9C2pQ4S3Y.png)


### Name


 Process Flow - Data Privacy Compliance - Access Renewal


### Description




### Reference(s)




## Element

[Expand all](#){ .md-button .diff-line }


### Timeline


    

<details markdown=1>
<summary markdown="span"></summary>

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
        <td></td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span"></summary>

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
        <td></td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
</table>


</details>


    



### Component Message


    

<details markdown=1>
<summary markdown="span">Save "no response" received</summary>

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
        <td>Save "no response" received</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>this means user continues using cogArch</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">[do not renew] delete architectures & personal info</summary>

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
        <td>[do not renew] delete architectures & personal info</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">[on completion of deletion] send notification</summary>

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
        <td>[on completion of deletion] send notification</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>will have to wait till backup deletes have been removed</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">[within 2 weeks] Respond</summary>

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
        <td>[within 2 weeks] Respond</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Compose renewal email</summary>

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
        <td>Compose renewal email</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Determine which users have to renew access</summary>

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
        <td>Determine which users have to renew access</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>To reconfirm user's usage annually.

Check for users who have used cogArch for a year minus 2 weeks.
</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Save renewal response</summary>

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
        <td>Save renewal response</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Save sent renewal email</summary>

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
        <td>Save sent renewal email</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>for each user</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Send renewal email</summary>

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
        <td>Send renewal email</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Options:
1) via email response with a Renew button
2) provide a link to a page with a Renew button/action</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

