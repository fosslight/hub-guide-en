---
sort: 10
published: true
---
# System (Admin Only)  
Check the FOSSLight Hub logs or change operational data.  
<br><br>

## Code Management  
{: .left-bar-title}  
<br>

Configure FOSSLight Hub operation-related settings.  
- You can search using Code No or Code Name (partial match supported).  
![config](images/9_system_code.png){: .styled-image}<br>  
- When you click a row in the search result list, detailed code information is displayed below.  
    - You can add a new row by clicking the + button at the top left of the table.  
    - You can also double-click a row in the list to switch it to edit mode.  
    - After making changes, click the Save button to apply the modifications.  
    - To cancel edit mode, reselect a row from the Code search result area. This will reset the detailed code section.  
![search](images/9_system_code_search.png){: .styled-image}     
<br><br><br>

## User Management  
{: .left-bar-title}
<br> 

Check and update the registered account information.  
- **Token Proc > Create** button: Generates a token to be used with the [REST API](https://fosslight.org/hub-guide-en/advanced/2_rest_api_2.html).  
- **Password > reset** button: Resets the password to the same value as the user ID.  
- **Use YN**: Sets the account as inactive.  
- **Admin**: Grants admin rights.  
![user](images/9_system_user.png){: .styled-image}  
<br><br><br>

## History List  
{: .left-bar-title}  
<br> 

View change history for License List, OSS List, and Project basic information.  
- **Search Area**  
    - **Name**: Search by License Name, OSS Name, or Project Name.  
    - **Modifier**: Search by user (action performer).  
    - **Modify Type**: Select License, Open Source, or Project to filter.  
    - **Action**: Select Insert, Update, or Delete to filter.  
    - **Modified Date**: Search change history within a specific period.  
![history](images/9_system_history.png){: .styled-image}  
- **Details**  
    - Double-click a row in the search result to check the details.  
![detail](images/9_system_history_detail.png){: .styled-image}   
<br><br><br>

## Notification  
{: .left-bar-title}
<br>

Manage the popup notification that appears when logging in to the FOSSLight Hub.  
![noti](images/9_system_noti_list.png){: .styled-image}  
- **Add**  
    - Click the + button at the top left to add a notification.  
    - **Start Date**: Notification start date  
    - **End Date**: Notification end date  
    - **Publish**: If checked, the notification popup is displayed  
![notiadd](images/9_system_noti_add.png){: .styled-image}  

- **Edit**  
    - Click the row of the notification you want to edit > click the icon at the top left ![notiicon](images/9_system_noti_modify_icon.png) > modify the content > click the Submit button.  
<br><br><br>

## Sent Mail List  
{: .left-bar-title}
<br>    

Check the mail sending history.  
![mail](images/9_system_mail.png){: .styled-image}  
<br><br><br>

## Vulnerability Log  
{: .left-bar-title}
<br>    

Check changes in OSS vulnerability data.  
- The vulnerability log is updated when OSS information is changed (e.g., nickname added), when a new vulnerability score is registered, or when a CVE ID with a higher score is added.  
- Use the filter function to check the change history of vulnerability information for a specific OSS (version).  
- Click the CVE ID to go to the CVE detail page on the NVD site.  
![vul](images/9_system_vul.png){: .styled-image}    
<br><br><br>

## Server Setting  
{: .left-bar-title }
<br>   

![server](images/9_system_server.png){: .styled-image}  

- **Authentication using LDAP**    
    - FOSSLight Hub supports user password authentication using LDAP via JNDI, in environments that support Active Directory or other LDAP servers.  
        - **Provider URL**: Set the LDAP server information in the format ldap://<AD_SERVER_IP>:<LDAP_PORT>. (javax.naming.Context.PROVIDER_URL)

- **Notice Setting**      
    - **Notice Type**: Set the type of OSS notice that can be issued.  
- **External Analysis Setting**  
    - In the Self-Check menu, configure the information for the FOSSLight Scanner Service that will be linked when analyzing the source code via the Upload URL.  
        - FL Scanner URL : Enter the URL of the FOSSLight Scanner Service server to be linked for analysis.  
        - Admin Token : Enter the token of an account with admin privileges. This token value must be the same as the one set in the FOSSLight Scanner Service.  
- **Workspace Path Setting**   
    - **Root Path**: Set the top-level workspace path for upload/download file storage.  
