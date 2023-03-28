

# AD-018


### Name

Leverage IBM Cloud PV Encryption to support data encryption at-rest for external version


### Status

accepted


### Last Update

2021-08-19


### Subject Area

Data Security At-Rest


### Topic




### Issue or Problem Statement

To protect users data in the Internet, the data stored in IBM Cloud must be encrypted at-rest


### Assumptions

<ul><li>Neo4j &amp; Mongodb Community version can not support data encryption at database level</li><li>There is no SPI  data in CogArch, like Bank Account, etc. <br></li></ul>


### Motivation

Support data encryption at-rest with the lowest application complexity &amp; better performance


### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Encrypt Data Encryption in the application </summary>

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
        <td>Encrypt Data Encryption in the application </td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>Provide framework in application to do the encrypt/decrypt on database data. <br></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>More secured, especially for SPI data</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><div><ul><li>Can not support partial query</li><li>Add the complexity on application</li><li>Impact on the performance<br></li></ul></div></td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Leverage IBM Cloud PV Encryption to support data encryption at-rest for external version</summary>

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
        <td>Leverage IBM Cloud PV Encryption to support data encryption at-rest for external version</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td>IBM Cloud provides the capability to encrypt PV by default. <br>For details, check the link <a href="https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-mng-data" target="_blank">https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-mng-data</a></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td><br><ul><li>    Has no impact on the application complexity</li><li>    Has no limitation on partial query</li></ul></td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td><ul><li>    Has dependency on IBM Cloud PV Encryption.</li></ul></td>
    </tr>
</table>


</details>


    



### Decision

Leverage IBM Cloud PV Encryption to support data encryption at-rest for external version


### Justification

<div>- No SPI data in IT Architect Assistant<br></div><div>- As PV Encryption is provided by IBM Cloud, can reduce the complexity at application level</div><div>- Without the encryption/decryption in the application, the performance will be better</div><div>- No Restriction on Application functions, like partial query.<br></div>


### Implications

- Needs the PV encryption capability provided by IBM Cloud
- The original encryption capability in application do no need to remove now, can keep there with configuration enable/disable


### Derived Requirements




### Related Decisions


