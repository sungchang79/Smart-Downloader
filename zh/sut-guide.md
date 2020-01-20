## Game > Smart Downloader > User Guide for Unity Tool 

## Getting Started 

Smart Downloader Unity Tool, or SUT is a tool to upload and deploy resources for Unity.  

### Environments

#### Supported Unity Versions

* 5.6.6 ~ 2019.2.17

### Download

[Smart Downloader Unity Tool](/Download/#game-smart-downloader)


### Install  

1. Open a Unity project. 
2. Go to **Assets > Import Package > Custom Package**.
3. Select and import 'Smart-downloader-unity-tool-{Version}.unitypackage', which is a downloaded Unity Tool file. 
    ![sut_import.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_import.png)

## Enabling Unity Tool  

To enable Unity Tool, go to menu and select **Tool > Toast > Smart Downloader > Unity Tool**. 

### Authenticate 

The **Authentication** tab shows if it is not yet authenticated. 

![sut_credentials_tab.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_credentials_tab.png)

* User ID: TOAST Cloud ID
* User Access Key ID, Secret Access Key
    1. Select **Issue User Access Key ID** from [API Security Setting](https://toast.com/account/api_settings).
    2. A window shows that Secret Access Key has been issued. 
    3. Check information and status of User Access Key ID that are issued from the API security setting page. 
    ![console_api_security_setting.png](https://static.toastoven.net/prod_smartdownloader/sut/console_api_security_setting.png)
* Project ID
    * A project ID using Smart Downloader can be found from **Project Setting** on console.  
    ![console_project_id.png](https://static.toastoven.net/prod_smartdownloader/sut/console_project_id.png)


### Query Services   

When it is authenticated, the **Upload** tab shows. 
Fill in **Appkey** and click **Query**, and it shows the list of services created on console.  

![sut_upload_tab_base.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_upload_tab_base.png)

* Appkey
    * Click **URL & Appkey** from Smart Downloader of the console and check issued appkey  
    ![console_appkey.png](https://static.toastoven.net/prod_smartdownloader/sut/console_appkey.png)

### Uploading Resources 

#### 1. Select Services 

Click a service to upload from the service list and select resource path. 
If the path is correct, the **Upload** button shall be activated. 

![sut_upload_step_1.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_upload_step_1.png)

#### 2. Select Upload Resources 

Compare resources of the selected path with those of the last uploaded, and show changes. Select resources to upload, and then, the **Upload** button shall be activated.  

> Caution 
Files that are automatically created from OS (.DS_Store, desktop.ini, thumbs.db) shall be excluded. 
Each resource cannot be larger than 5GB. 

![sut_upload_step_2.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_upload_step_2.png)

#### 3. Upload Resources 

Shows uploading progress. 
If tool is closed while uploading is underway, a window pops up asking whether to cancel uploading or not. 

> Caution 
Do not force close unity while uploading is underway. 
If it is forced to close, the status remains to be uploading, and will be changed to failure in 30 minutes.  

![sut_upload_step_3.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_upload_step_3.png)


#### 4. Complete

When it is normally completed, a windows pops up to confirm. 

![sut_upload_step_4.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_upload_step_4.png)


### Service Details 

Select service from the list and double-click to show **Service Details**. 

![sut_service_detail_info.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_service_detail_info.png)

* Service Information
    * Service Name: Name of service entered for service registration.
    * Service Description: Description of registered service.
    * CDN Address: Address with which CDN is completely integrated.
* Most Recent Uploads 
    * Date and Time: The last upload time and date of resources.
    * Last Registrant: User ID uploading resources.
    * Upload Resource Information: Number and total size of uploaded resources.
        * Detail Information: Uploaded resource information.
    * Deployment Status: Check status of deployment. See [Console User Guide](http://docs.toast.com/zh/Game/Smart%20Downloader/zh/console-guide/#4-list-of-services) for deployment status. 
        * Updates: Upload service details.  
        * Build Deployment: To be activated when build is ready to be deployed, with the latest build deployed by CDN. 
* Build Deployment History: Shows the history of the most recent 10 build deployment cases.  


#### Build Deployment 

![sut_service_detail_info_deploy.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_service_detail_info_deploy.png)

* Only when the deployment status is **Ready for Deployment, or Deployment Failed**, the most updated upload resources can be deployed to CDN.  

### Settings 

![sut_settings.png](https://static.toastoven.net/prod_smartdownloader/sut/sut_settings.png)

* Version Data: Shows the version information of Unity Tool. 
* Change of Language: Change the language for the tool: Korean, English, and Japanese are supported. 