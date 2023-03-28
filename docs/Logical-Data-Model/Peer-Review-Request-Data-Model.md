

## Diagram

![Peer Review Request Data Model](../img/logicalerd_HkygqnpXVBnt.png)


### Name


Peer Review Request Data Model



### Description




### Reference(s)




## Element

[Expand all](#){ .md-button .diff-line }


### Entities


    

<details markdown=1>
<summary markdown="span">Architecture</summary>

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
        <td>Architecture</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>CastSolutionId,</strong>[String]</div>
                <div></div>
                
                <div><strong>Created,</strong>[Date]</div>
                <div></div>
                
                <div><strong>Description,</strong>[String]</div>
                <div></div>
                
                <div><strong>IbmInternal,</strong>[String]</div>
                <div></div>
                
                <div><strong>IsAsIs,</strong>[Boolean]</div>
                <div></div>
                
                <div><strong>LastModified,</strong>[Date]</div>
                <div></div>
                
                <div><strong>LastModifiedUserId,</strong>[String]</div>
                <div></div>
                
                <div><strong>Name,</strong>[String]</div>
                <div></div>
                
                <div><strong>NumOfCopied,</strong>[Integer]</div>
                <div></div>
                
                <div><strong>OriginalType,</strong>[String]</div>
                <div></div>
                
                <div><strong>RankValue,</strong>[String]</div>
                <div></div>
                
                <div><strong>SalesConnectNum,</strong>[String]</div>
                <div></div>
                
                <div><strong>Status,</strong>[String]</div>
                <div></div>
                
                <div><strong>Type,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">CAUser</summary>

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
        <td>CAUser</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>avatar,</strong>[]</div>
                <div></div>
                
                <div><strong>chatbotToken,</strong>[]</div>
                <div></div>
                
                <div><strong>email,</strong>[]</div>
                <div></div>
                
                <div><strong>focusRole,</strong>[]</div>
                <div></div>
                
                <div><strong>fullname,</strong>[]</div>
                <div></div>
                
                <div><strong>jobResponsibilities,</strong>[]</div>
                <div></div>
                
                <div><strong>lastLoginDate,</strong>[]</div>
                <div></div>
                
                <div><strong>notesId,</strong>[]</div>
                <div></div>
                
                <div><strong>password,</strong>[]</div>
                <div>placeholder will not store it</div>
                
                <div><strong>username,</strong>[]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">PeerReviewRequest</summary>

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
        <td>PeerReviewRequest</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>PeerReviewRequest in Mongo <div>(ca-db-user or a new db)</div></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>archId,</strong>[String]</div>
                <div></div>
                
                <div><strong>businessProblem,</strong>[String]</div>
                <div></div>
                
                <div><strong>coreTechElements,</strong>[String]</div>
                <div></div>
                
                <div><strong>created,</strong>[Date]</div>
                <div></div>
                
                <div><strong>expireDate,</strong>[Date]</div>
                <div>To get all expired request in batch job, the expiration should be date time, but not in days.</div>
                
                <div><strong>manualExpireDate,</strong>[Date]</div>
                <div>If this request is expired by request owner manually, then save the date of this manual expiration request.</div>
                
                <div><strong>requestOwner,</strong>[String]</div>
                <div></div>
                
                <div><strong>type,</strong>[String]</div>
                <div>pre-sale<div>delivery</div></div>
                
                <div><strong>_id,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">RequestCollection</summary>

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
        <td>RequestCollection</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>ca-db-history</td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>date,</strong>[Date]</div>
                <div></div>
                
                <div><strong>requestOwnerList,</strong>[List]</div>
                <div></div>
                
                <div><strong>_id,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">RequestOwnerInfo</summary>

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
        <td>RequestOwnerInfo</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>ca-db-history</td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>requestOwner,</strong>[String]</div>
                <div></div>
                
                <div><strong>reviewArchList,</strong>[List]</div>
                <div></div>
                
                <div><strong>_id,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">ReviewArchInfo</summary>

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
        <td>ReviewArchInfo</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>ca-db-history</td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>archId,</strong>[String]</div>
                <div></div>
                
                <div><strong>commentCount,</strong>[Integer]</div>
                <div></div>
                
                <div><strong>_id,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    



### Relationships


    

<details markdown=1>
<summary markdown="span">Aggregate</summary>

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
        <td>Aggregate</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
            </td>
        
    </tr>
    <tr>
        <td> <strong>Relationship Connections</strong> </td>
        
        <td>
                
                <div><strong>1,</strong>[1]</div>
                <div>RequestCollection</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>PeerReviewRequest</div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Create</summary>

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
        <td>Create</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
            </td>
        
    </tr>
    <tr>
        <td> <strong>Relationship Connections</strong> </td>
        
        <td>
                
                <div><strong>1,</strong>[1]</div>
                <div>CAUser</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>PeerReviewRequest</div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Relationship</summary>

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
        <td>Relationship</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
            </td>
        
    </tr>
    <tr>
        <td> <strong>Relationship Connections</strong> </td>
        
        <td>
                
                <div><strong>1,</strong>[1]</div>
                <div>RequestCollection</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>RequestOwnerInfo</div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Relationship</summary>

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
        <td>Relationship</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
            </td>
        
    </tr>
    <tr>
        <td> <strong>Relationship Connections</strong> </td>
        
        <td>
                
                <div><strong>*,</strong>[*]</div>
                <div>ReviewArchInfo</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>RequestOwnerInfo</div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Relationship</summary>

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
        <td>Relationship</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
            </td>
        
    </tr>
    <tr>
        <td> <strong>Relationship Connections</strong> </td>
        
        <td>
                
                <div><strong>1,</strong>[1]</div>
                <div>Architecture</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>PeerReviewRequest</div>
                
            </td>
        
    </tr>
</table>


</details>


    

