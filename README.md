# AzureSphereExplorer_SPA
Run the AzureSphereExplor for SPA.
Base Project is [ms-identity-javascript-v2](
https://github.com/Azure-Samples/ms-identity-javascript-v2).

# Prerequisites
* You have an account for azure sphere tenant.
* You have an azure sphere tenant.
* Google Chrome Browser.
* Google Chrome Plugin [Allow CORS](
https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf).
* Nginx.

# Runnning the Demo
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
2. Run the Google Chrome Brouser and Allow CORS plugin valid.  
3. Sign in to your azure sphere tenant.  
4. Select tenant.  
