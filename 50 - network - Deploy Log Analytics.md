

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
# Install the Web Session Essentials Solution
