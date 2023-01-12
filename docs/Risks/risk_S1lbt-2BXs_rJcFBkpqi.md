

# R-001 Reusing ODM subscription for multi-tenants

### Risk Description


Assessment must be done when new tenants are onboarded to the Customs Compliance Platform. The outcome of this assessment could be that one ODM on Cloud subscription will be used by multiple tenants.
This decision raises the following risks that must be considered:
1. Tenants will share the same ODM on Cloud infrastructure. This means that in case of increased load of any of the tenants, other tenants could be impacted. Note: ODM on Cloud doesn't have auto-scaling capabilities
2. Increased load during black week for all tenants could impact the performance




### BU / Department / Competency




### Owner




### Probability


High



### Impact


High



### Effort / Cost




### Contingency / Mitigation recommendation


1. Detailed analysis for tenants loads and volumes must be done before taking the decision of sharing one ODM subscription<div>2. This decision must be revisited before black week or any period with expected high load</div>



### Date Raised




### Review Date




### Date Closed




### Comments




### Is this a Key Risks?

true


### External



