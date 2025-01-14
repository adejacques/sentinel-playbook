# Run QuevlarAi Investigation after Azure Sentinel Incident creation
author: QevlarAi

This playbook is triggered by a Microsoft Sentinel newly created Incident. It creates a new Investigation by Qevlar AI and insert a new comment in the Incident with the result of the Investigation.  

## Prerequisites

Before deploying the the playbook you will need to:
- Set the required permissions 

## Quick Deployment
[Learn more about playbook deployment](https://github.com/Azure/Azure-Sentinel/tree/master/Playbooks/ReadMe.md)

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fadejacques%2Fsentinel-playbook%2Fmaster%2Fazuredeploy.json)
[![Deploy to Azure Gov](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazuregov.png)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fadejacques%2Fsentinel-playbook%2Fmaster%2Fazuredeploy.json)

## Post-Deployment
[Learn more about automation rules](https://docs.microsoft.com/azure/sentinel/automate-incident-handling-with-automation-rules#creating-and-managing-automation-rules)

After deployment, attach this playbook to an **automation rule** so it runs when the incident is created.