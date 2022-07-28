# Business Add-In Implementation

You need to implement the enhancement spot and the BAdI: Online Check BAdI for each validation. 

To create a BAdI implementation, proceed as follows:
1. Go to the SE19 transaction.
2. In the Create Implementation section, select the New BadI option and enter OVS_ENH_CHECK in the Enhancement Spot field. 
3. Select Create.
Enter the name of the enhancement spot and BAdI as needed. 

## Implementation Class
You can use the following example of a implementation class as a reference when creating the BAdI:
```
ZCL_OVS_EXAMPLE
```
which can be found [here](../src/zcl_ovs_example.clas.abap). 

When you have created the BAdI implementation, enter a BAdI filter (case sensitive) just as the example below:
```
CHECK_ID = <your_check_id>
```
The filter value must be equal to the previously defined CheckID.

Example
![BAdI filter](img/BAdI_Filter.png)