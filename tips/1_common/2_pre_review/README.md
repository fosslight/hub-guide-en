---
sort: 2
published: true
---

# Reviewing Open Source by Download Location (Pre-Review)
<div class="note">
º Using the Pre-Review button, you can retrieve Open Source information or License information stored in the system based on the Download Location.<br>
º It can be used for Project and 3rd Party Identification, as well as for Self-Check.<br>
<img src="../../images/common/pre_review/pre_review.png" />
</div>

## Check the OSS Name
{: .left-bar-title }
<div class="note">
It can suggest the OSS name based on the specified download location.
</div>

#### How to check the OSS Name
{: .under-bar-title}
1. Click on Pre-Review > Open Source.    
2. Select the row you want to change to the ‘Registered OSS Name (to be changed)' value.   
3. Click ‘Change OSS Name'. The changed Open Source name will be reflected in the OSS Table.   
<div style="margin-left: 20px;">
    <img src="../../images/common/pre_review/pre_review_opensource.png" alt="PreReview_oss" class="styled-image" />
</div>

#### Pre-Review Table Detailed Features
{: .under-bar-title}
- If the specified download location is redirected, a recommended OSS Name (Registered OSS Name) will be generated based on the redirect URL, and you can check the redirect URL information at the bottom.
  <div style="margin-left: 20px;">
    <img src="../../images/common/pre_review/pre_review_redirect_url.png" alt="PreReview direct url" class="styled-image"/>
  </div>
- If the download location is inaccessible, a warning message <span style="color:red">Invalid download location.</span> will be displayed in ‘Registered OSS name (to be changed)'.  
  <div style="margin-left: 20px;">
    <img src="../../images/common/pre_review/pre_review_redirect_url.png" alt="PreReview direct url" class="styled-image" />
  </div>
- Clicking on the recommended OSS Name will show detailed information about that OSS.<br><br> 
- If a row is displayed in gray, it means that more than one OSS was found for the same download location. You can click the cell of the Registered OSS Name to select the OSS Name you want to change.  
  <div style="margin-left: 20px;">
    <img src="../../images/common/pre_review/pre_review_multi_recommand.png" alt="PreReview multi recommand" class="styled-image" />
  </div>
- Changes made by clicking ‘Change OSS Name' or ‘Change License' will be immediately reflected in the OSS Table and recorded in the ‘Comment'. You can check the change history through the ‘Comment'.  
<br><br><br><br>

## Check License
{: .left-bar-title }
<div class="note">
You can check the declared licenses based on Download Location, OSS Name, and OSS Version.  
</div><br>

#### How to check the License
{: .under-bar-title}  
1. Click on Pre-Review > License.  
2. Select the row you want to change to the ‘License (to be changed)' license.  
3. Click ‘Change License'. The changed license will be reflected in the OSS Table.  
<div style="margin-left: 20px;">
    <img src="../../images/common/pre_review/pre_review_license.png" alt="PreReview License" class="styled-image"/>
</div><br><br><br><br>

## (Admin Only) Modifying Open Source Information     
{: .left-bar-title }
<div class="note">
º The buttons 'Add Nickname - OSS name(now)' and 'Add URL, Nickname based on URL' are only visible to Admins.<br>
º You can modify the Open Source information listed in the 'Registered OSS name (to be changed)'. However, this is only possible if the 'Registered OSS name (to be changed)' is registered in the database, and no additional information will be added for already saved entries.
</div><br>

#### Adding Nickname or Nickname and URL to Open Source  
{: .under-bar-title} 
1. Click on Pre-Review > Open Source.  
2. Select the row of the Open Source information you want to modify. The Open Source that is to be modified is the one listed under the 'Registered OSS Name (to be changed)' column.  
3. Click 'Add Nickname - OSS name(now)'. The value of 'OSS name(now)' will be added as the nickname for the selected Open Source. If you want to add both the nickname and the URL simultaneously, click the 'Add URL, Nickname based on URL' button.  
<img src="../../images/common/pre_review/pre_review_nickname.png" alt="pre_review_nickname" class="styled-image" /> 

#### Pre-Review Table Detailed Features  
{: .under-bar-title}
- If the specified download location is redirected, a recommended OSS Name (Registered OSS Name) is generated based on the redirect URL, and you can check the redirect URL information at the bottom.    
- If the download location is inaccessible, a warning message Invalid download location. will be displayed under 'Registered OSS name (to be changed)'.   
- Clicking on the recommended OSS Name will show detailed information about that OSS.   
- If a row is displayed in gray, it means that more than one OSS was found for the same download location. You can click the cell of the Registered OSS Name to select the OSS Name you want to change.   
- Changes made by clicking 'Change OSS Name' or 'Change License' will be immediately reflected in the OSS Table and recorded in the 'Comment'. You can check the change history through the 'Comment'.    