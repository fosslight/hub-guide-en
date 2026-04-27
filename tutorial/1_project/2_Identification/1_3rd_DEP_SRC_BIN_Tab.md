---
sort: 1
published: true
---

# 3rd Party/DEP/SRC/BIN Tab
<div class="note">
Upload the analysis report or load a confirmed Project or 3rd Party.
</div>  

## Process
{: .left-bar-title }
- Upload the result of [FOSSLight Scanner](https://fosslight.org/fosslight-guide-en/scanner/) analysis
- [**Check Warning message**](https://fosslight.org/hub-guide-en/tips/1_common/5_warning_message)

## Fill in OSS List in the browser
{: .left-bar-title }
Click the + button at the top-left of the OSS Table to fill OSS information.

## Upload Analysis Report
{: .left-bar-title }
1. Click the + button in the upload area. (First time: go to step 2.)
<img src="images/1_upload_report1.png" alt="select" class="styled-image">
2. Select 'Upload Analysis Result', then click the Upload button to upload the FOSSLight Report file.  
Reports in Excel, SPDX, and CycloneDX formats can be uploaded.
<img src="images/1_upload_report2.png" alt="select" class="styled-image">
3. Left: sheet list. Right: select the tab to upload to.  
One sheet per tab; sheets starting with the tab name are selected by default. Uncheck sheets you don't want to load.
<img src="images/1_select_sheet.png" alt="select" class="styled-image">
4. When you click Save, the data from the uploaded report file is loaded into the OSS Table below and saved.

## Project/3rd Party Search
{: .left-bar-title }
Load a confirmed Project or 3rd Party.

1. Click the + button in the upload area. (First time: go to step 2.)
<img src="images/1_upload_report1.png" alt="select" class="styled-image">
2. Select Project Search or 3rd Party Search.
Search for the Project or 3rd Party to load by Project/3rd party Name or ID.
<img src="images/1_project_search.png" alt="select" class="styled-image">
<img src="images/1_3rd_search.png" alt="select" class="styled-image">
3. Select the tab to load. Data loads only into the tab with the same name (e.g., SRC → SRC tab).
<img src="images/1_select_tab.png" alt="select" class="styled-image">
4. When you click Save, the data of the selected project/3rd party is loaded into the OSS Table below and saved.


## Display of Uploaded / Loaded Data
{: .left-bar-title }
<img src="images/1_loaded_item.png" alt="select" class="styled-image">
1. Loaded 3rd party
2. Loaded project
3. Uploaded report file
4. Total : Number of uploaded report files and loaded projects and 3rd parties
OSS Components : Number of OSS components loaded in each tab

<img src="images/1_oss_component_comment.png" alt="select" class="styled-image">
- The origin is displayed in the Comment column of the OSS Table.

## Delete
{: .left-bar-title }
<img src="images/1_delete1.png" alt="select" class="styled-image">

1. Select a single row you want to delete and click the trash can icon. The following pop-up will appear.
<img src="images/1_delete2.png" alt="select" class="styled-image">
2. When you click OK, the selected row is deleted and all OSS Table data loaded from that row is deleted and saved.
3. If nothing is selected or more than one row is selected, the following pop-up will appear.
<img src="images/1_delete3.png" alt="select" class="styled-image">

## Reset
{: .left-bar-title }
<img src="images/1_reset1.png" alt="select" class="styled-image">
1. Click the Reset button.
2. A pop-up will appear indicating that all uploaded and loaded rows will be selected and all data will be deleted.
<img src="images/1_reset2.png" alt="select" class="styled-image">
3. When you click OK, all selected rows are deleted, all data in the OSS Table is deleted, and the changes are saved.
4. To reset each tab individually, click the reset button located within the corresponding tab.
