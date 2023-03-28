

# AD-020


### Name

Decouple CA frontend to multiple code repos


### Status

proposed


### Last Update

2022-01-11


### Subject Area

Micro-frontend


### Topic

Frontend Architecture


### Issue or Problem Statement

Current develop and release model/process can not support rapid release.  Since frontend is a single big web application,  code change of stories are mixed and may have conflict. Also test and regression scope is not clear.


### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Decouple frontend to multiple web repositories</summary>

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
        <td>Decouple frontend to multiple web repositories</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><img style="height: 418.993px; width: 748.993px;" src="../../files/file_d4eb861bc8d97d11.png"><div><b>Pros</b>
</div><div><ol><li>physically decouple one big web app to several small ones with separate repo
</li><li>can develop/deploy individual application
</li><li>clear test/regression scope (per application)
</li></ol></div><div><b>Cons</b>
</div><div><ol><li>need effort to update devpos to support multiple applications build and version management
</li><li>page navigiation between application is not smooth
</li><li>multiple page resource load (per application for 1st time)
</li><li>contain reduntant code
</li><li>complicated invocation between applications and hard to share data
</li><li>effort to convert single application to multiple ones</li></ol></div></td>
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
<summary markdown="span">One web repository and leverage multiple branches to release story</summary>

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
        <td>One web repository and leverage multiple branches to release story</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><img style="height: 395.989px; width: 766.987px;" src="../../files/file_eed5c3ef93e9e116.png"><div><b>Pros</b>
</div><div><ol><li>Single web application: smooth page navigation
</li><li>Single web application: one-time page resource load
</li><li>Easily to reuse components (inside one application) and no redundant code 
</li></ol></div><div><b>Cons</b>
</div><div><ol><li>it's risky having more other code update than planned stories
</li><li>it's risky having the wrong test/regression scope per human evaluation
</li><li>code merge between branches could bring issues: code conflict and lost
</li><li>need repeat test after code merge
</li><li>need to deploy whole application for any release</li></ol></div><div><br></div></td>
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

Decouple frontend to multiple web repositories


### Justification

<ol><li>Physically code repository isolation is more important for 1)developer: not impact other story development; 2) test: clear test/regression scope</li><li>Frequent code merge for stories is not good to bring code conflict and lost</li></ol>


### Implications




### Derived Requirements




### Related Decisions


