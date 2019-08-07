# Sentia
This template creates: 
An Azure Datalake Gen 2 storage account.
A key vault with a secret
A virtual network
A web app that can access both the datalake storage and the key vault secret
Tags to group the resources. 


Assumptions:
1. There should be an already created App Service Plan in the subscription. The template needs it as a parameter to perform correctly. 
2. I chose a Web App resource (App service), which I believe that it includes a built in internet facing loadbalancer. So in my opinion, I don't see a need to create a new one using the template.
3. In order for the web app to access the storage and the key vault, i used network service endpoints feature.
3. The tag that i used for all resources is : Sentia :Prod.
