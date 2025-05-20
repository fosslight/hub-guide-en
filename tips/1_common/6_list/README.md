---
sort: 6
published: true
---

# Common Features in the List View

## Export Project Search Results  
{: .left-bar-title }
- Click the <img src="../../images/common/list_view_buttons/list_export_icon.png" width="20" height="20" alt="Add" /> button at the top left of the list to export the currently displayed search results in each menu as an Excel file.  
- The total number of search results is shown at the bottom right.  
- Export is not available for results exceeding 5000 items.  
- **Main Menus**  
    - Open Source  
    - License  
    - Project  
    - 3rd party  
    - Self-Check  

<img src="../../images/common/list_view_buttons/list_export.png" width="700" height="400" alt="ListExport" class="styled-image" />  
<br><br><br>

## Change Division, Edit Permission, and Status  
{: .left-bar-title }  
- You can use the Change button at the top of the menu to change the information of the selected projects.   
- You must have Edit Permission for the selected projects to make changes.  
- **Main Menus**: Project, 3rd Party (Status change not available)  
<img src="../../images/common/list_view_buttons/list_changes.png" width="600" height="400" alt="ListChange" class="styled-image" />   

### Change Division  
{: .specific-title }  
- You can change the Division of multiple projects at once.  
- **How to change**  
  1. Select the projects that you want to change > Click the Change button > Click Division.  
  2. Choose the new Division and click OK.  
    <img src="../../images/common/list_view_buttons/change_division_popup_1.png" alt="ChangeDivisionPopup_1" class="styled-image" />  
  3. Click the OK button again.  
    <img src="../../images/common/list_view_buttons/change_division_popup_2.png" width="350" height="120" alt="ChangeDivisionPopup_2" class="styled-image" />  
    If even one of the selected projects does not have Edit Permission, a popup will display the project ID without permission, and the Division will not be changed.    
   <img src="../../images/common/list_view_buttons/change_division_popup_3.png" width="350" height="120" alt="ChangeDivisionPopup_3" class="styled-image" />       

### Change Edit Permission  
{: .specific-title }
- You can add or remove Edit Permissions for multiple projects at once.  
- **How to change**  
  1. Select the projects > Click the Change button > Click Edit Permission.  
  2. Select the user to be added as Edit Permission and click the <img src="../../images/common/list_view_buttons/status_edit_2_icon.png" width="40" height="25" alt="Add" /> button.  
   <img src="../../images/common/list_view_buttons/change_edit.png" width="500" height="150" alt="ChangeEditPermission" class="styled-image" />  
    - **Select Division**: You can select the users by Division.  
    - **Input AD ID**: You can enter an AD account and select the domain to add a user.  
  3. Click the <img src="../../images/common/list_view_buttons/status_edit_add_icon.png" width="40" height="20" alt="Add" /> button and then click OK.  
  To remove existing Edit Permission users, select the users and click the <img src="../../images/common/list_view_buttons/change_edit_delete_icon.png" width="40" height="20" alt="Add" /> button.  

### Change Status  
{: .specific-title }
- You can change the Status of a project.  
- **How to change**  
  1. Select the projects you want to change the Status from the project lists.  
  2. Click the Change button > Click Status.  
  3. Select the Status you want to change to, enter the reason, and click OK.  
   <img src="../../images/common/list_view_buttons/change_status.png" width="350" height="300" alt="ChangeStatus" class="styled-image" />  

- **Available Status Types**  
  - The available Status types differ depending on the user's role.   
    - **General User**: You can change project Status to Drop or Restart Identification.    
    - **Admin**: You can change project Status to Drop, Restart Identification, or Complete.    
<br><br><br>

## Custom Columns  
{: .left-bar-title }  
- In each menu's list view, you can customize and save the columns displayed in the list view individually.    
![ChangeDivisionInList](../../images/common/list_view_buttons/custom_columns.png){: .styled-image}  

- **Applicable Menus**  
  - License  
  - Open Source  
  - Project  
  - 3rd party  
  - Self-Check  
<br>

- **Default Columns**  
  The default column settings for each menu are as follows.
  - **License**: License Name, Restriction, Notice, Source  
  - **Open Source**: ID, OSS Name, OSS Version, License Name, Notice, Source  
  - **Project**: ID, Project Name, Status, OSC Process, Download  
  - **3rd party**: ID, 3rd Party Name, Software Name (Version), Status  
  - **Self-Check**: ID, Project Name (Version)  
<br>

- **How to Add or Remove Columns**  
  - Click the ![ChangeDivisionInList](../../images/common/list_view_buttons/custom_columns_button.png) button at the top left of the grid > Select or deselect the columns you want > Click Save.  
  - The selected columns will be saved and loaded the next time you log in.
