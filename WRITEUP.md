# Write-up Template

The followings are analysis of VM and App service when it comes to decide which solution is right for the CMS app:
*VM
    - Cost: Running VMs, in general, is more expensive then running Azure App Service. But VMs provide pay-as-you-go model, while App service does not.
    - Scalability: in terms of scalability, VMs are better at scaling, both vertically and horizontally than App service. this is because VM instance is not hardware limited as app service.
    - Availability: VM conectivity varies from 95% to 99.99% depending on the setting of the VM and how VMs scaling.
    - Workflow: Develop an application in VMs is labor intensive than App service because developers have to take care of many part of the app like OS, runtime ...

*VM
    - Cost: App service is cheaper than VM. But App service does not provide pay-as-you-go model, no matter how many instances is running, we have to pay for the app service plan
    - Scalability: app service instance is limited by maximum 14 GB memory and 4 CPU core per instance
    - Availability: App service connectivity is guranteed to stay at 99.95% all the time
    - Workflow: Develop an application in App service is easier because it supports Continous deployment and developers do not have to take care about underlying things like OS, runtime ...
*I choose App Service for the CMS app because of the following reasons:
    - although App service does not provide pay-as-you-go model, it 's still cheaper and  for a light weight app like CMS app, we don't need an app plan that is too power.
    - because CMS app is a simple app and light weight, there no need to scale it well and App service connectivity is good enough.
    - Deploy the CMS app to App service is easier and less labor intensive than VMs.

*Belows are some factors that might change my decision in the future:
    - Developers are required to deploy the CMS to a dedicated server due to security reason.
    - the CMS app owner want to control the full server access.
    - the CMS users increase rapidly.

URL to the active CMS app :
https://huynhnn-cms-udacity.azurewebsites.net


