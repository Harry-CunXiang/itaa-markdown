

# System Availability


### ID

NFR-01


### Name

System Availability


### Description

Provides high availability based on current infrastructure & middleware limitation


### Theme


Availability



### Context


1. Currently, neo4j is using community version, could not support hot backup. But it is critical to backup users' latest 7 days data
2. Bluecloud has the periodical maintenance time
3. CogArch deployment requires downtime to deploy new version. 



### Value




### Growth Rate




### Acceptance Criteria


1. 15 minutes downtime every day for data backup
2. Additional downtime caused by the bluecloud maintenance or new release/patch deployment. 
3. Support blue-green deployment for new version deployment.
Less than 2 hours downtime for deployment without data migration
Less than 4 hours downtime for deployment with data migration





### Priority


Critical



### Source




### Reference


JIRA: https://jsw.ibm.com/browse/IIAA-1288?jql=text%20~%20%22NFR%22



### Test Method


Resilience Test
1. Break down part of the service instance to check the availability
2. Chaos/Monkey Test



### Owner




### Review Date

2021-04-07
