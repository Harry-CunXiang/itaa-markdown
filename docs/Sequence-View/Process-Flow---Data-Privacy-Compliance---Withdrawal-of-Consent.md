

## Diagram

![Process Flow - Data Privacy Compliance - Withdrawal of Consent](../img/cmdynamicview_rkuskl3pQVS3F.png)


### Name


Process Flow - Data Privacy Compliance - Withdrawal of Consent


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
<summary markdown="span">[For private architectures with Collaborators] Notify collaborators
 (via email)</summary>

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
        <td>[For private architectures with Collaborators] Notify collaborators
 (via email)</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>For any private architectures that have collaborators, notify either of deletion or change of ownership</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Acknowledge Cancellation request (via email)</summary>

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
        <td>Acknowledge Cancellation request (via email)</td>
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
<summary markdown="span">Acknowledge Withdrawal request has completed (via email)</summary>

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
        <td>Acknowledge Withdrawal request has completed (via email)</td>
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
<summary markdown="span">Acknowledge 
Withdrawal request (via email)</summary>

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
        <td>Acknowledge 
Withdrawal request (via email)</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Within 7 days of receiving request, send acknowledgement with the following info:
- All architectures in cogArch will be deleted which include private and curated ones.
- Once deleted, the architectures cannot be restored and will no longer be available.
Deletion will be completed in 48-72 hours (configurable) unless otherwise notified to cancel the withdrawal.

Deletion of the architectural assets will include deletion of PI (Name and email address).
</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Cancel withdrawal request</summary>

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
        <td>Cancel withdrawal request</td>
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
<summary markdown="span">Compose email - acknowledgement of withdrawal request</summary>

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
        <td>Compose email - acknowledgement of withdrawal request</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>include:
- list of architectures
- ownership reassignment</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Compose email - arch content</summary>

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
        <td>Compose email - arch content</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>include:
- list of architectures
- ownership reassignment</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Delete curated architectures</summary>

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
        <td>Delete curated architectures</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>including user information</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Delete private architectures</summary>

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
        <td>Delete private architectures</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>including user information</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Delete user from collaboration architectures</summary>

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
        <td>Delete user from collaboration architectures</td>
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
<summary markdown="span">Determine user architecture list</summary>

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
        <td>Determine user architecture list</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>including user information

list of architectures includes :
- private
- curated
- share as-is
- collaboration

</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Initiate Cancellation request</summary>

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
        <td>Initiate Cancellation request</td>
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
<summary markdown="span">Initiate Withdrawal 
request</summary>

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
        <td>Initiate Withdrawal 
request</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Execute within 7 days of receipt of request.
Provide user email, request date.

-> invoke API to set user for withdrawal</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Notify cancellation of withdrawal</summary>

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
        <td>Notify cancellation of withdrawal</td>
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
<summary markdown="span">Send confirmation notice</summary>

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
        <td>Send confirmation notice</td>
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
<summary markdown="span">Send email to request confirmation</summary>

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
        <td>Send email to request confirmation</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Include a link to a page with the following:
- list of curated and share as-is architectures
- option to change ownership for above listed architectures
- confirmation button of changes made

Inform user they have to make the changes within 48-72 hours (configurable), else all will be deleted with no re-assignment of ownership.</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Send Withdrawal 
email request</summary>

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
        <td>Send Withdrawal 
email request</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>User sends email to cogarch@us.ibm.com to request withdrawal from cogArch.</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Set confirmation request</summary>

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
        <td>Set confirmation request</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>includes re-assignment of ownership where applicable</td>
    </tr>
    <tr>
        <td> <strong>Type</strong> </td>
        <td>Call</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Update confirmation request</summary>

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
        <td>Update confirmation request</td>
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


    

