

# Deploy Log Analytics
# Create a Data Collection Endpoint
# Collect IIS Logs
# Enable Sentinel
# Install the Web Session Essentials Solution




# Deploy Log Analytics

<img width="1074" height="600" alt="image" src="https://github.com/user-attachments/assets/b51d2f27-a9d0-487c-87ae-421ba7ebcc03" />




<img width="994" height="412" alt="image" src="https://github.com/user-attachments/assets/46aedece-e126-4eba-95ef-2cd404be07de" />



```

Deploy Log Analytics
From the top search bar, search for and navigate to Log Analytics workspaces.
Click Create Log Analytics workspace.
Leave Subscription as its default and select the only option for the Resource group.
For the Instance details section:
Enter the exact name log-sentinel into the Name field
Set the Region field to match the region for the existing resources
Click Next: Review + create.
Click Create.
```



# Create a Data Collection Endpoint




<img width="1029" height="510" alt="image" src="https://github.com/user-attachments/assets/58188e4e-02e5-45d9-878b-aca3302e0679" />



```
From the top search bar, search for and navigate to Data Collection Endpoints.
Click Create Data collection endpoint.
For the Endpoint details section:
Enter any name into the Name field, e.g. dce-log-sentinel
Leave Subscription as its default
Select the only option for the Resource group
Set the Region field to match the region for the existing resources
Click Next: Review + create.
Click Create.
Note: Wait for the deployment of the Data Collection Endpoint and Log Analytics workspace before continuing.

```





# Collect IIS Logs


<img width="578" height="84" alt="image" src="https://github.com/user-attachments/assets/b2e94028-a8d6-4404-b132-4e143a2b57d8" />

<img width="883" height="639" alt="image" src="https://github.com/user-attachments/assets/706b3d1a-516e-463c-8065-41e4f8a9ea52" />

We need to add resources
<img width="1908" height="578" alt="image" src="https://github.com/user-attachments/assets/2b4865e9-54cf-4a49-8afb-17b4e25d8702" />

<img width="1922" height="591" alt="image" src="https://github.com/user-attachments/assets/27680fa2-5c27-4ea0-9a92-449c0ceed788" />

<img width="1862" height="504" alt="image" src="https://github.com/user-attachments/assets/07cd44a7-7b4c-4bef-a05d-82c40be2713e" />







<img width="1173" height="940" alt="image" src="https://github.com/user-attachments/assets/c8836a4e-2aa9-4772-9846-c638d8061183" />


```
Collect IIS Logs
From the top search bar, search for and navigate to Data Collection Rules.
Click Create data collection rule.
For the Rule details section:
Enter any name into the Name field, e.g. dcr-collect-iis-logs
Leave Subscription as its default
Select the only option for the Resource group
Set the Region field to match the region for the existing resources
Set the Platform Type field to Windows
Select the only option for the Data Collection Endpoint, which should be the Data Collection Endpoint you created in the previous step
Click Next: Resources.
Click + Add resources.
Select webserver1 from the list of available resources
Click Apply
Select Enable Data Collection Endpoints.
Select the only option for the data collection endpoint for the virtual machine
Click Next: Collect and Deliver >.
Click + Add data source.
On the Data source tab, set the Data source type to IIS Logs
Click Next: Destination >.
The Destination details will be pre-filled with your existing Log Analytics workspace
Click Add data source
Click Next: Review + create.
Click Create.
```


# Enable Sentinel





<img width="962" height="271" alt="image" src="https://github.com/user-attachments/assets/1e5fb4b6-0599-4aef-a013-529d22f28ad4" />

<img width="1226" height="404" alt="image" src="https://github.com/user-attachments/assets/aa29cf12-b7db-44ef-9709-6a4099806bb6" />





# Install the Web Session Essentials Solution


## Content Hub place with rules ??? 


```
Install the Web Session Essentials Solution
From the left menu, under Content management, select Content hub.

In the search bar, type and select Web Session Essentials.

On the right information panel, click Install.

Wait for the content to be installed.

Note: For the real world, just be aware that we've already configured log collection from our webserver, so we don't need to configure a data connector, but many other solutions will require a Data connector to be configured after installing the solution
```
