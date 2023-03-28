

## Diagram

![Architecture Data Model - Collaboration Diagram](../img/logicalerd_S1uep36mNBhF.png)


### Name


Architecture Data Model - Collaboration Diagram



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
<summary markdown="span">CM Collaboration Diagram</summary>

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
        <td>CM Collaboration Diagram</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>Description,</strong>[string]</div>
                <div></div>
                
                <div><strong>Name,</strong>[string]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">ComponentEvent</summary>

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
        <td>ComponentEvent</td>
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
                
                <div><strong>number,</strong>[]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Entity</summary>

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
        <td>Entity</td>
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
<summary markdown="span">Logical Component</summary>

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
        <td>Logical Component</td>
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
                
                <div><strong>Level,</strong>[String]</div>
                <div></div>
                
                <div><strong>Name,</strong>[String]</div>
                <div></div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Logical Participant</summary>

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
        <td>Logical Participant</td>
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
</table>


</details>


    



### Relationships


    

<details markdown=1>
<summary markdown="span">Connectors</summary>

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
        <td>Connectors</td>
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
                <div>ComponentEvent</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>CM Collaboration Diagram</div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Participants</summary>

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
        <td>Participants</td>
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
                <div>CM Collaboration Diagram</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>Logical Participant</div>
                
            </td>
        
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">REF</summary>

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
        <td>REF</td>
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
                <div>Entity</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>ComponentEvent</div>
                
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
                <div>ComponentEvent</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>Logical Participant</div>
                
            </td>
        
    </tr>
</table>


</details>


    

