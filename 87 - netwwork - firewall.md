# Fromm Resources group
Create Firewall fromm Market

<img width="1104" height="596" alt="image" src="https://github.com/user-attachments/assets/853c265d-8058-4400-8f45-3ef1a365afb8" />

Deploy Azure Firewall
From the resource group navigate to the Create button in the action menu.

Search Firewall in the Marketplace.

Create a Firewall using the Azure Firewall service tile.

Set the following values:

Resource group: Select the existing one in the dropdown.
Name: Enter fw-01.
Note: The name fw-01 is used to grade the lab.

Region: Select the same region as the lab-provided resource group
Firewall SKU: Select Basic.
Firewall management: Select Policy-based.
Policy: Click Add new, name it fwpolicy-01, select the same region as the lab-provided resource group, and click OK.
Note: The name fwpolicy-01 is used to grade the lab.

Choose a virtual network: Select Use existing.
Virtual network: Select the existing one in the dropdown.
Public IP address: Click Add new, name it pip-fw-01, and click OK.
Management Public IP address: Click Add new, name it pip-mgmt-fw-01, and click OK.
Click Review + create.

Click Create.

Note: It may take up to 45 minutes for the deployment to complete. So you will come back to this later on in the lab.




![Uploading image.png…]()




