

## Diagram

![Cognitive Search Data Model](../img/logicalerd_SJj0K3a74H2Y.png)


### Name


Cognitive Search Data Model



### Description




### Reference(s)




## Element

[Expand all](#){ .md-button .diff-line }


### Entities


    

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
<summary markdown="span">Cooccurrence</summary>

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
        <td>Cooccurrence</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>category_of_label,</strong>[String]</div>
                <div></div>
                
                <div><strong>co_occurrence_items,</strong>[Array]</div>
                <div></div>
                
                <div><strong>label,</strong>[String]</div>
                <div></div>
                
                <div><strong>number_of_label,</strong>[Int]</div>
                <div></div>
                
                <div><strong>original_label,</strong>[String]</div>
                <div></div>
                
                <div><strong>_id,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Feedback</summary>

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
        <td>Feedback</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>archId,</strong>[]</div>
                <div></div>
                
                <div><strong>comments,</strong>[]</div>
                <div></div>
                
                <div><strong>relevence,</strong>[]</div>
                <div></div>
                
                <div><strong>userId,</strong>[]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">ModelOverView</summary>

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
        <td>ModelOverView</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>record model training status</td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>lastUpdateFinishDate,</strong>[Date String]</div>
                <div>for example: 2021-09-24 05:03:01</div>
                
                <div><strong>lastUpdateStartDate,</strong>[Date String]</div>
                <div>for example: 2021-09-24 05:03:01</div>
                
                <div><strong>ModelName,</strong>[String]</div>
                <div>Co-occurrence</div>
                
                <div><strong>status,</strong>[String]</div>
                <div>In Progress/Completed/Failed</div>
                
                <div><strong>_id,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">ProcessedLabelsInCoModel</summary>

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
        <td>ProcessedLabelsInCoModel</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>category_of_original_label,</strong>[String]</div>
                <div></div>
                
                <div><strong>category_of_processed_label,</strong>[String]</div>
                <div></div>
                
                <div><strong>embedding_vector,</strong>[Array]</div>
                <div></div>
                
                <div><strong>original_label,</strong>[String]</div>
                <div></div>
                
                <div><strong>processed_label,</strong>[Array]</div>
                <div></div>
                
                <div><strong>sentence_embedding_vector,</strong>[Array]</div>
                <div></div>
                
                <div><strong>_id,</strong>[]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Query</summary>

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
        <td>Query</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>text,</strong>[]</div>
                <div></div>
                
                <div><strong>type,</strong>[]</div>
                <div></div>
                
                <div><strong>_id,</strong>[]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    



### Relationships


    

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
                <div>Query</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>CAUser</div>
                
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
                <div>Query</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>Feedback</div>
                
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
                <div>Cooccurrence</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>ProcessedLabelsInCoModel</div>
                
            </td>
        
    </tr>
</table>


</details>


    

