

# System Security


### ID

NFR-02


### Name

System Security


### Description

Provides security mechanism for internal or external users


### Theme


Security



### Context


1. Need to meet the GDPR requirement, especially do not store users SPI information
2. Transformation message needs to be encrypted
3. External version database data needs to encrypted



### Value




### Growth Rate




### Acceptance Criteria


1. CA does not store users' SPI information, users authentication/authorization will target to W3ID(Internal) 
2. The transformation layer is using SSL
3. Static & Dynamic Code Scan, major above issues need to be fixed
4. SPbD Cafetiere Meet



### Priority


Critical



### Source




### Reference


JIRA: https://jsw.ibm.com/browse/IIAA-1290?jql=text%20~%20%22NFR%22



### Test Method


Security Test, Maintainability test
1.	Verify service communication should use HTTPs
2.	Verify all network traffic encrypt
3.	Should meet GDPR requirement
4.	DB encrypted for external db data
5.	Transformation message need to be encrypted
6.	Verify the audit log and log for security events and threats




### Owner




### Review Date

2018-09-30
