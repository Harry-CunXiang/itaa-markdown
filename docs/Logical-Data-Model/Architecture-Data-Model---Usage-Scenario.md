

## Diagram

![Architecture Data Model - Usage Scenario](../img/logicalerd_HyHQK3am4rhF.png)


### Name


Architecture Data Model - Usage Scenario



### Description




### Reference(s)




## Element

[Expand all](#){ .md-button .diff-line }


### Entities


    

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
<summary markdown="span">Logical Connection</summary>

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
        <td>Logical Connection</td>
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
<summary markdown="span">Usage Scenario</summary>

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
        <td>Usage Scenario</td>
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
<summary markdown="span">Usage Step</summary>

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
        <td>Usage Step</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td></td>
    </tr>
    <tr>
        <td> <strong>Attributes</strong> </td>
        
        <td>
                
                <div><strong>Step_Description,</strong>[String]</div>
                <div></div>
                
                <div><strong>Step_Label,</strong>[String]</div>
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
                <div>Usage Scenario</div>
                
                <div><strong>*,</strong>[*]</div>
                <div>Usage Step</div>
                
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
                <div>Usage Step</div>
                
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
                <div>Usage Step</div>
                
                <div><strong>1,</strong>[1]</div>
                <div>Logical Connection</div>
                
            </td>
        
    </tr>
</table>


</details>


    

