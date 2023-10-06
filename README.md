# INTEGRA Geschaeftspartner mutieren

Link to INTEGRA master repository  
[INTEGRA](https://github.com/Integra-SUPERB/INTEGRA)


## Goal of this repository
With the Geschäftspartner mutieren API, existing business partners can be modified. The API behaves identically in many parts to the [Geschäftspartner anlegen](https://github.com/Integra-SUPERB/INTEGRA_Geschaeftspartner-anlegen) API. 

For more information on the functionality of the API, you can consult the description and the XML of the [Geschäftspartner anlegen](https://github.com/Integra-SUPERB/INTEGRA_Geschaeftspartner-anlegen) interface.


## How does this API work?
As already mentioned, there is only a small difference between the "Geschäftspartner mutieren" and [Geschäftspartner anlegen](https://github.com/Integra-SUPERB/INTEGRA_Geschaeftspartner-anlegen) interfaces; additionally, some attributes must be provided for the mutation to work.

On the <BusinessPartner> tag, the following attributes must be provided:

`BusinessPartner reconciliationPeriodCounterValue="1"`  
`addressInformationListCompleteTransmissionIndicator="true"`  
`commonListCompleteTransmissionIndicator="true"`  
`roleListCompleteTransmissionIndicator="true"`  
`identificationListCompleteTransmissionIndicator="true"`  

**Important:** Please note that from the sender's perspective, the OUT interfaces are always used. Middleware maps the information from OUT to IN and makes the data available for further processing.

How the OUT (outbound) replication is handled is described by SAP here: [Replicate request out service](https://api.sap.com/api/CO_MDG_BP_RPLCTRQ/resource).

For information on IN (inbound) replication, SAP provides further information here: [Replicate request in service](https://api.sap.com/api/OP_BUSINESSPARTNERSUITEBULKREPLIC/resource?ReleaseInfo=2022%20FPS00)


## Contact information
With the information provided above, you should gain a high-level overview of the capabilities of the API. 

If you wish to use and work with the API, please contact us so that we can review your application and provide you with the necessary credentials and information.

For further assistance with the API, the BIT technical support SAP team is available to answer your questions during normal office hours.

To contact us, please email FachsupportSAP@bit.admin.ch
