---
sort: 2
published: true
---
# License
```note
You can check registered license information and add, modify, or delete licenses.
You can check detailed information by clicking a cell in the License Name Column of the License List.
```
## License List
![LicenseList](images/3_lic_list.PNG)

### License Name
- The License Full name follows the SPDX notation (<https://spdx.org/licenses/>).
- If you click the value of the License Name column, you can check detailed information for each license.

### Identifier
- The standardized short identifier makes it easier to identify the License and follows the SPDX notation (<https://spdx.org/licenses/>).

### License Type
- **Permissive**
    - Known as BSD-like or BSD-style License, it has minimal requirements for software distribution.
    - Typically, it is required to maintain the copyright notice and disclaimer.
- **Weak Copyleft**
    - You can freely distribute copies and modified versions of the work on the condition that the same rights are retained in the derivative work. 
    - Source codes of copies and revisions of the work must be disclosed.
- **Copyleft**
    - You can freely distribute copies and modified versions of the work on the condition that the same rights are maintained in the derivative work. 
    - Not only copies and revisions of the work, but also the source code of the entire program linked to or operating with it must be disclosed.
- **Proprietary**
    - Since it cannot be used without the permission of the software right holder, be sure to check the contractual relationship with respect to the use of the source code before using it.
- **Proprietary Free**
    - No additional contract is required, but can be used in a restricted form, specific terms and conditions or conditions.

### Restriction

|**Restriction Type**|**Description**|
|-----|---|
|**Non-Commercial Use Only**|Commercial use and distribution of software is prohibited. <br> ex) CC-BY-NC-X.X|
|**Network Redistribution**|Just providing a service for use on a network is regarded as distribution, and the obligations of open source must be fulfilled. <br> ex) AGPL-3.0, OSL-2.0|
|**No Modification**|You cannot distribute a modified version of the software. That is, it should be used without modifying the source code. <br> ex) CC-BY-ND-X.X|
|**Platform Limitation**|Software distribution is restricted according to the operating system, technology, technology field used, and device type. <br> ex) Amazon Software License (must be used for web services, computing platforms, or applications provided by Amazon.com or its subsidiaries)|
|**Prohibited Purpose**|Software cannot be used for a specific purpose(field). <br> ex) The Happy Bunny License (cannot be used for military purposes)|
|**Specification Constraints**|Software should be used in relation to a specific specification or standard. <br> ex) ETCPACK Software License Agreement (It can be used for compression and/or decompression according to the Khronos standard specifications) |
|**Redistribution Restriction**|Restricted software sub-components (Source Code, Binary file, etc.) that can be redistributed. <br> ex) SOFTWARE LICENSE FOR VIVANTE CORPORATION (TM) USER SPACE GRAPHICS DRIVER BINARY (can only be redistributed in binary form|
|**Contract Required**|It cannot be used without a commercial contract, with control over the use of the source code. <br>ex) QT Commercial License, NVIDIA Commercial License|
|**Internal Use Only**|It allowed only for internal use. <br> ex) Additional-Buildcraft-Objects-Mod License|
|**No Charge**|It cannot be used if a fee is charged. <br> ex) Commons Clause License Condition v1.0, SIL Open Font License 1.1|
|**No Change the Name**|This license does not allow to change name. <br> ex) IPA Font License|
|**Provide Installation Information Required**|It must provide installation information. <br> ex) GPL-3.0|
|**Patent Warning**|This license may be subject to patent disputes and should be used with caution. <br> ex) Apple Public Source License|
|**Semi-Copyleft**|This license has restrictions, but there are no problems with use if the source code is disclosed. <br> ex) Ruby License|
|**Contact Required**|This license must be verified by contacting the copyright holder.|
|**Unexpected Termination**|The license may be terminated at any time by the copyright holder.|
|**Use Restriction**|There are restrictions on use, such as the number of users, country of use, and others.|

### Obligation
You can find out the notice and source code disclosure obligations for each license.
- **Notice Obligation**(<img src="images/6_self_check_notice_icon.PNG" width="20" height="20" />): Obligation for OSS Notice
- **Source Code Obligation**(<img src="images/6_self_check_src_icon.PNG" width="20" height="20" />): Obligation for distributing Source Code.

### Web site
- Provides web site information of the original license. Click the URL to go to the site.

### User Guide
- You can see the precautions when using the license.

## (Admin Only) Add, Modify, Delete License
### Add
![NEW_OSS](images/3_lic_add.PNG)
1. Click the Add button in the upper right of the License List.
2. At the "New_License" tab, enter the information of the new OSS.
    - **License Name** and **Nick Name** cannot be duplicated.
    - **Obligation** :
        - If Notice is checked, it is included in the OSS Notice.
        - If Source Code is checked, it is displayed as a list of source code collection OSS in the Packaging tab.
    - **User Guide** : Enter information about the OSS.
    - **Attribution** : When issuing an OSS Notice, enter the phrase that must be included separately.
3. Click the Save button(<img src="images/save_button.PNG" width="20" height="20" />) at the top right.

### Modify
1. In the License List, click the License Name to be modified.
2. Make modifications on the License Details tab.
3. Click the Save button at the top right.

### Delete
1. In the License List, click the license name you want to delete.
2. In the License Details tab, enter the reason for deletion in the Comment field.
3. Click the Delete button at the top right.