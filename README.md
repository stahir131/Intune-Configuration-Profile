<p align="center">
  <h4>Intune Configuration Profile</h4>
</p>

Device profiles allow you to add and configure settings, and then push these settings to devices in your organization. You have some options when creating policies:

  <b>Administrative Template</b>: These settings allow administrators to create group policies using the cloud.


Using the Administrative template, I have setup the following settings for OneDrive and assigned it a device group:

  <b> 1.Use OneDrive Files On-Demand</b>: This setting tells OneDrive to keep the data in the cloud and just set up the file and folder structure - files that users open will be downloaded on demand.

<b>2.Silently sign in users to the OneDrive sync client with their Windows credentials</b>: When using Azure AD Join or Hybrid Azure AD Join, the Azure AD user token is already available and can be used to automatically sign into OneDrive for Business

<b>3.Silently sign in users to the OneDrive sync client with their Windows credentials:</b> When using Azure AD Join or Hybrid Azure AD Join, the Azure AD user token is already available and can be used to automatically sign into OneDrive for Business

Sign in to Office 365 as global or SharePoint admin
Go to <b>Endpoint manager</b> -> Windows Devices -> Configuration profiles -> Create policy -> Windows 10 and later

Profile type: Template -> Administrative template -> Create

Give it a name: OneDrive sync -> Next > Choose <b>OneDrive</b>

Search for the 3 settings above to enable them.

Scope tag -> Default 

Assignments -> I have assigned this to the dynamic group I have created, “All Windows Devices”

The config. looks like this before creation.

![OneDrive1](https://github.com/stahir131/Intune-Configuration-Profile/assets/64047385/95faeccf-a686-4ccf-b6be-777714cbdb76)

![OneDrive1](https://github.com/stahir131/Intune-Configuration-Profile/assets/64047385/95faeccf-a686-4ccf-b6be-777714cbdb76)


