# Deploy the VM-Series Firewall on Azure in Germany


This template launches the VM-Series in Germany to be deployed with all of the necessary hardware components needed to operate the VM-Series. By default in other regions the VM-Series is deployed with the following three separate interfaces. 

- Mgmt interface  eth0
- Untrust Interface eth1
- Trust interface eth2

However, in Germany the interfaces aren't created as a part of the deployment at this time. To assist with this we have provided this ARM deployment template to provide all of the resources needed to launch your VM-series in Germany. You can launch this template by clicking the deploy button below. You will still need to configure your VM-Series because this ARM template doesn't bootstrap any default configuration. Once you have launched your VM-Series and configured the firewall it will function as normal. 

Note: If you plan to connect your untrust interface directly to the internet you will need to create a public IP address and associate this IP address your untrust interface. After associating this interface if you are unable to reach the interface and your firewall is fully configured, please restart your firewall. 


[<img src="http://azuredeploy.net/deploybutton.png"/>](https://portal.microsoftazure.de/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fpaloaltonetworks%2Fazure-germany%2Fmaster%2Fazuredeploy.json) 


