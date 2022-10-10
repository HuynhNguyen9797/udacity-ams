# Write-up Template

For the CMS app, both a VM and an App Service have their pros and cons:
    - Both VM and App Service provides high availability and scalability
    - VM: Developers has multipe choice for hardware solution than App Service. In addition, developers can fully control the VM 's access, choose the image that they think will fit their use case. But using VM is quite expensive, developing the CMS app, which is light weight, to a VM is quite cumbersome so i think VM is not the right choice for this situation.
    - App service: while App service has its own limitations like hardware limitation, not full control access to the server, i think App Service is the best choice for the CMS app. it 's less expensive, easier for devs to develop because it supports Continous Deployment. App Service fits the best for a light weight app like the CMS app. 
    So i choose App Service for the CMS app.

Belows are some factors that might change my decision in the future:
    - Developers are required to deploy the CMS to a dedicated server due to security reason.
    - the CMS app owner want to control the full server access.
    - the CMS users increase rapidly.

URL to the active CMS app :
https://huynhnn-cms-udacity.azurewebsites.net


