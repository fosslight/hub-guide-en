---
sort: 4
published: true
---
# Project
<div class="note">
The process required for the development and distribution of software that includes open source software is carried out sequentially.<br><br>
    1. <strong>Identification</strong>: OSS Report Registration <br>
    2. <strong>Approval</strong>: OSS Report Review <br>
    3. <strong>Package Verification</strong>: Collecting Packages and Generating OSS Notice

</div>

<iframe width="560" height="315" src="https://www.youtube.com/embed/IUrQyj3s-Ps" title="FOSSLight Hub - 프로젝트 생성" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Project List
{: .left-bar-title }
You can search for a project, check the overall information of the project, and download the FOSSLight Report, OSS Notice, and OSS Package.
![ProjectList](images/4_project_list_main.png){: .styled-image}  

### 1. Project Search
{: .specific-title}  
- You can search by the project's name. With **Advanced Search** feature, you can search using various conditions.
    - Advanced Search
        - You can search under various conditions such as ID, Creator, Model Name, etc.
     ![Project_adv_search](images/4_project_search_adv.png){: .styled-image}


### 2. Project ID
{: .specific-title}  
- It is a unique number that identifies the project.

### 3. Projcet Name (Version)
{: .specific-title}  
- Double-clicking a row takes you to the project detail screen.

### 4. Status
{: .specific-title}  
- It displays the status information of the project.

|Status|   Description   |
|----|----|
|<span style="color:green"> Progress </span>| The user is currently writing.|
|<span style="color:pink"> Request </span>| The user has requested a review in the Identification or Packaging stage. <br>The status can be changed to Progress using Self Reject.|
|<span style="color:orange"> Review </span>| The reviewer is currently reviewing in the Identification or Packaging stage. <br>The user cannot modify the project information. <br>If modifications are needed, please leave a [Comment](#comment) for the reviewer to request a reject.|
|<span style="color:purple"> Final Review </span>| The OSPO manager is conducting the final review.|
|<span style="color:black"> Complete </span>| It means the project review is complete. <br>The user cannot modify the project information.<br> If modifications are needed, please request a reopen from the reviewer.|
|<span style="color:grey"> Drop </span>| It means the OSC process is no longer being carried out. <br> If it is not in the Complete status, the user can drop it regardless of the status, <br>and if necessary, they can click Reopen to open it again.|


### 5. OSC Process
{: .specific-title}  
- It indicates the progress stage of the project's OSC process.
    - Identification -> Packaging -> Distribution
- The color of the process stage changes based on the status.


### 6. Download
{: .specific-title}  
- (<img src="images/4_project_download_report_icon.PNG" width="20" height="25" />): You can download the list entered in Identification in the **FOSSLight Report**.
- (<img src="images/4_project_download_file_icon.PNG" width="20" height="25" />): If the source code to be released is uploaded in Packaging, an icon will be displayed, and you can download **the OSS Package file**.
- (<img src="images/4_project_download_notice_icon.PNG" width="20" height="25" />): When the Packaging stage is completed, an icon will be displayed, and you can download **the OSS Notice**.


### 7. Security
{: .specific-title}  
<div class="note">
In the Security tab, you can check and manage the status of actions for each CVE ID for OSS with a vulnerability score above the threshold based on the BOM tab in the Identification stage.<br>
    • The threshold for the Vulnerability Score can be set in Code Management > 760 (Security Vulnerability Score).
</div>

![prj](images/4_project_sec_list.PNG){: .styled-image}
- It displays the Vulnerability information for the entire open source list included in the Identification stage (except the ones that 'Exclude' is checked).
    - (<img src="images/4_project_security_need_to_resolve.PNG" width="120" height="25" />) : If the vulnerability score is above the threshold
    - (<img src="images/4_project_security_na.PNG" width="120" height="25" />) : If the vulnerability score is below the threshold


#### Columns
{: .under-bar-title}
- **OSS Name, OSS version**
    - The OSS information entered in the BOM tab of the Identification stage is automatically displayed.
- **CVE ID, CVSS Score, Published Date**
    - The CVE ID and the corresponding CVE ID's CVSS Score and published date information are automatically displayed.
- **Vulnerability Resolution**
    - The default value is set to Unresolved, and it can be changed to Fixed when the security vulnerability is resolved.

#### If OSS version is not entered
{: .under-bar-title}
- In the Security tab, it is difficult to accurately verify vulnerabilities for CVE IDs without an OSS version, so the entire list of CVE IDs is not displayed.
- If the following popup screen appears when entering the tab, you can view the accurate list of security vulnerability CVE IDs in the Security tab after entering the correct version of the corresponding open source in the Identification tab and saving the BOM tab.    
![prj](images/4_project_sec_popup.PNG){: .styled-image}

#### Reflecting Vulnerability Resolution in the Identification Stage
{: .under-bar-title}
- When checking the vulnerability score in the Identification stage tab, you can see the excluded max score for CVE IDs whose vulnerability resolution value has been changed to 'Fixed' in the Security tab.
- When clicking the Vulnerability Icon in the Identification stage tab, you can see that the 'Fixed' CVE IDs are deactivated in the entire CVE ID list window for the corresponding OSS name and version, as shown below.
![fixed](images/4_project_security_fixed.png){: .styled-image}
<br>
