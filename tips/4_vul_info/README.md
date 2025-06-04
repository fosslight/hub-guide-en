---
sort: 4
published: true
---

# Tips: Vulnerability 
It provides information on collecting vulnerability data, notifications, and how to display scores.
<br><br>  

## Vulnerability Data Collection  
{: .left-bar-title }  
- Vulnerability data is downloaded daily from the [NVD Data Feed](https://nvd.nist.gov/vuln/data-feeds) and stored in the FOSSLight Hub.
- The Vulnerability Score in the FOSSLight Hub is primarily based on the CVSS v3 Base Score, and if the v3 Score is not available, the CVSS v2 Base Score is used instead.  
<br><br><br>  

## Vulnerability Notification  
{: .left-bar-title }  
- An alert email will be sent when a Vulnerability Score that exceeds the threshold is registered for the first time, or when a Vulnerability Score changes from above the threshold to below it.
    - If an OSS that meets the above conditions is included in the BOM of a Project with confirmed Identification, the Vulnerability Score change will be sent to the Project's Creator, Edit Permission, and Reviewer.  
    - If you no longer wish to receive alert emails, you can [change the Security Mail (Vulnerability) setting to Disable in Project Information](https://fosslight.org/hub-guide-en/tips/4_vul_info/#security-mailvulnerability).  
<br><br><br>  

## Vulnerability Score Display Method  
{: .left-bar-title }  
- If there is a Vulnerability with the same OSS Name/Nickname and Version entered by the user, the Max Score of that OSS will be displayed.
    - If there is a Vulnerability for the OSS Version entered by the user, the Max Score of that Vulnerability will be displayed.
    - If there is no Vulnerability for the OSS Version entered by the user, it will not be displayed as there is no value.
    - If the user leaves the OSS Version blank, the Max Score among all Versions of that OSS will be displayed.
- If the OSS Name is '-', no Vulnerability will be displayed.
<br><br><br>

## Security Mail (Vulnerability)  
{: .left-bar-title }  
You can enable or disable the receipt of Security Mail (Vulnerability).  

### Security Mail (Vulnerability) Settings
{: .specific-title}
- If you set Security Mail (Vulnerability) in Project Information to **Disable**, no further Vulnerability emails will be sent for that Project.
- A reason must be provided when setting it to Disable.  
![vul_mail_setting](../images/vulnerability/vul_mail_setting.png){: .styled-image} 

### Searching Security Mail (Vulnerability) Settings 
{: .specific-title}
 - You can search for the Security Mail (Vulnerability) setting value (Enable or Disable) in the Project List.  
![vul_mail_search](../images/vulnerability/vul_mail_search.png){: .styled-image}