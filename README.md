# AzureSphereExplorer_SPA
Run the AzureSphereExplor for SPA demo.
Base Project is [ms-identity-javascript-v2](
https://github.com/Azure-Samples/ms-identity-javascript-v2).

# Content
|  File name  |  Description  |
| ---- | ---- |
|  authConfig.js  |  Settings for Azure Sphere Public API.  |  
|  authPopup.js  |  Main authentication logic resides here (using Popup flow).  |
|  azurePublicAPI.js  |  Using Azure Sphere Public API.  |
|  main.js  |  Main method. |
|  ui.js  |  Contains UI logic.  |
|  index.css  |  CSS file for index.html  |
|  index.html  |  Index file.  |


# Prerequisites
* You have an account for Azure Sphere tenant.
* You have an Azure Sphere tenant.
* Using a browser where you can set up a Allow CORS. e.g.Google Chrome.
  * Installed Google Chrome Browser. 
  * Installed Google Chrome Plugin [Allow CORS](
https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf).
* Using a web server where you can set up a reverse proxy. e.g. Nginx.
  * Installed Nginx.

# Running the Demo
1. Setup Nginx.  
1.1 Set Reverse Proxy in nginx.conf.  
```
http {
 server {
  location / {
#  root   html;
#  index  index.html index.htm;
   proxy_pass https://reikayamazaki.github.io/AzureSphereExplorer_SPA/; 
  }
 }
}
```
1.2 Run the Nginx.  
2. Run the Google Chrome Browser and enable Allow CORS plugin.  
3. Access http://localhost/.  
4. Sign in to your account for Azure Sphere tenant.  
5. Select a tenant and click the [Select] button.  
6. Click product name in Product or device group name in Device Group.
