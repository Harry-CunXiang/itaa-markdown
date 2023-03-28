

# Risk-02 Instance Update Mechnism Limitation


### Risk Description


To provide better user experience, currently, the instance update mechanism is batch update, that means every instance updates(user click Save or Auto-Save in front-end) might include a lot of cascade updates/delete operations in one single transaction. Along with the data becomes more complex, the code maintenance will be a challenge.



### BU / Department / Competency




### Owner




### Probability


High



### Impact


Medium



### Effort / Cost


Code Refine Effort / Testing Effort



### Contingency / Mitigation recommendation


<div>1. Provides the UT with high coverage on different cascade updates/delete operations in one transaction.<br></div><div>2. In the future, reduce each instance/element update api granularity to reduce the complexity. This may influence user experience, so need to consider the balance while do the refine. And consider to use Web Socket solution<br></div>



### Date Raised




### Review Date

2019-01-01


### Date Closed




### Comments




### Is this a Key Risks?

true


### External


