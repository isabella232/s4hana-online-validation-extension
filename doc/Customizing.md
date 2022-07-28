# Configuration for Online Validation

## Create a Definition for Your Validation

Define the check ID, maintain the result codes, and enable selective online validation in Customizing for Cross-Application Components under SAP Business Partner -> Online validation -> Maintain Online Validation Checks (transaction OVS_CHECKS). 

### Define Check IDs
Create the main record for your Validation.

| Field Name | Description |
| ----------- | ----------- |
| Check ID | ID of the check. It must start with Z or Y. The rest of the ID can be chosen freely.  |
| Validity of Check Result| It defines how many days can be an existing result returned again without a need to validate online. |
| Check ID description | Human readable name. It will appear in F4 Helps |

### Maintain Result Codes
Create as many various result codes as required by the business. 
Note that SAP recommends to maintain at least the following result codes: 

| Result Code | Description |
| ----------- | ----------- |
| 1 | Valid | 
| 2 | Invalid | 
| 3 | Valid, Internal result exists  | 
| 4 | Validation Disabled | 
| 5 | Technical error | 

## Enable Selective Online Validation
Here you can enable or disable the validation execution in each supported business process. To enable the validation in certain process, this table must contain a row for given Integration spot and the checkbox must ticked. 
| Field Name | Description |
| ----------- | ----------- |
| Integration Spot | Name of the business process |
| Enable | If checked, the validation will be enabled | 


## Create an Remote Function Call (RFC)
You need an RFC communication for a connection with an external service. 


### Online Validation
Go to the SM59 transaction and create an RFC to the desired service. 
Make sure you create the parameters for the RFC according to the documentation of the online service. 


## Configure the Online Validation with the New RFC
Once you have created the RFC, maintain the RFC to the respective check ID in Customizing for Cross-Application Components under SAP Business Partner -> Business Partner -> Basic Settings -> Online Validation -> Activate Validation Checks (transaction OVS_CHECKACTIV). 

Note that the name of the RFC is case-sensitive and must be maintained as in transaction SM59.
Once you have maintained the RFC, this validation will be executed. To avoid any issues when running your business processes, make sure to do this step when the implementation is ready for testing. 

For more information about how to maintain this Customizing activity, check the documentation in the system.


## Offline Validation
If your validation does not communicate with an external service, maintain an entry with the Check ID and empty RFC in Customizing for Cross-Application Components under SAP Business Partner -> Business Partner -> Basic Settings -> Online Validation -> Activate Validation Checks (transaction OVS_CHECKACTIV). 