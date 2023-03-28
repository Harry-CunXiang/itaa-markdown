

## Diagram

![Architecture Data Model - Enterprise View](../img/logicalerd_BJJPY3aQVH3t.png)


### Name


Architecture Data Model - Enterprise View



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
<summary markdown="span">Enterprise View</summary>

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
        <td>Enterprise View</td>
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


    

<details markdown=1>
<summary markdown="span">SubSystem</summary>

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
        <td>SubSystem</td>
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
                
                <div><strong>*,</strong>[*]</div>
                <div>Logical Participant</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>SubSystem</div>
                
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
                <div>Logical Participant</div>
                
                <div><strong>1,</strong>[1]</div>
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
                <div>Enterprise View</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>SubSystem</div>
                
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
                <div>ComponentEvent</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>Enterprise View</div>
                
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
                <div>Enterprise View</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>Logical Participant</div>
                
            </td>
        
    </tr>
</table>


</details>


    

