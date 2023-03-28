

## Diagram

![Architecture Data Model - Use Case Text](../img/logicalerd_SJtNF3TmVB3Y.png)


### Name


Architecture Data Model - Use Case Text



### Description




### Reference(s)




## Element

[Expand all](#){ .md-button .diff-line }


### Entities


    

<details markdown=1>
<summary markdown="span">Actor</summary>

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
        <td>Actor</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>Description,</strong>[String]</div>
                <div></div>
                
                <div><strong>Name,</strong>[String]</div>
                <div></div>
                
                <div><strong>Type,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Association</summary>

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
        <td>Association</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>Description,</strong>[String]</div>
                <div></div>
                
                <div><strong>Name,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use Case</summary>

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
        <td>Use Case</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>Alternative_Flows,</strong>[String]</div>
                <div></div>
                
                <div><strong>Basic_Flow,</strong>[String]</div>
                <div></div>
                
                <div><strong>Description,</strong>[String]</div>
                <div></div>
                
                <div><strong>Failure_Outcomes,</strong>[String]</div>
                <div></div>
                
                <div><strong>Name,</strong>[String]</div>
                <div></div>
                
                <div><strong>PackageName,</strong>[String]</div>
                <div></div>
                
                <div><strong>Preconditions,</strong>[String]</div>
                <div></div>
                
                <div><strong>Successful_outcome,</strong>[String]</div>
                <div></div>
                
                <div><strong>UCID,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">UseCaseText</summary>

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
        <td>UseCaseText</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>Description,</strong>[String]</div>
                <div></div>
                
                <div><strong>Name,</strong>[String]</div>
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
                
                <div><strong>1,</strong>[1]</div>
                <div>Use Case</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>Association</div>
                
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
                <div>Actor</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>Association</div>
                
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
                <div>UseCaseText</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>Association</div>
                
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
                <div>Actor</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>UseCaseText</div>
                
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
                <div>UseCaseText</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>Use Case</div>
                
            </td>
        
    </tr>
</table>


</details>


    

