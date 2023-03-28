

# AD-023


### Name

Use Instana as Monitor Tool


### Status

proposed


### Last Update

2022-02-26


### Subject Area

Monitor


### Topic

Monitor Tool Choose


### Issue or Problem Statement




### Assumptions




### Motivation




### Notes



[Expand all](#){ .md-button .same-line }


### Alternatives


    

<details markdown=1>
<summary markdown="span">Use Instana as Monitor Tool</summary>

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
        <td>Use Instana as Monitor Tool</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><ul><li>Infrastructure Monitor: Basic cpu, memory, disk usage, network, tcp connection</li><li>Cluster Monitor: Support</li><li>Service Monitor: Service discovery auto, api response time for each service.</li><li>Website Monitor: Monitor page load time, error on client side.</li><li>Troubleshooting: Error Analysis.</li><li>Migration: Need installation, configuration for internal staging/prod is ready.</li></ul></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>Instana provides more useful function on service level, it can help us more for monitoring and troubleshooting.</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>Infrastructure level is not good, especially on Network monitor</td>
    </tr>
</table>


</details>


    

<details markdown=1>
<summary markdown="span">Use sysdig as Monitor Tool</summary>

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
        <td>Use sysdig as Monitor Tool</td>
    </tr>
    <tr>
        <td> <strong>Description</strong> </td>
        <td><ul><li>    Infrastructure Monitor: Basic cpu, memory, disk usage, network, tcp connection, and also support I/O Monitor</li><li>    Cluster Monitor: Support</li><li>    Service Monitor: No</li><li>    Website Monitor: No</li><li>    Troubleshooting: No</li><li>    Migration: Provided by IBM cloud, no action for installation, only need to do configuration.</li></ul></td>
    </tr>
    <tr>
        <td> <strong>Best Applied</strong> </td>
        <td>Sysdig provides more capability on Infrastructure Monitor</td>
    </tr>
    <tr>
        <td> <strong>Contraindications</strong> </td>
        <td>No Service, Website and Troubleshooting capability</td>
    </tr>
</table>


</details>


    



### Decision

Use Instana as Monitor Tool


### Justification

1. Instana is good at service dependency(api calls among different services) and error analysis.<br>2. Instana provides websites monitor(brownser), it can help us to analyze user behaviour and Front-end Errors.


### Implications

1. Needs to request process and configure Instana to IBM Cloud



### Derived Requirements




### Related Decisions


