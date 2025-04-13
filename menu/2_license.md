---
sort: 2
published: true
---
# License
<div class="note">
º You can check the registered license information, and by clicking on the License Name, you can view the detailed information for that specific license.<br>
º (Admin Only) You can add, modify, or delete a license.
</div>

## License List
{: .left-bar-title }
![LicenseList](images/3_lic_list.png)

### License Name
{: .specific-title} 
- The License Full Name follows the SPDX notation (<https://spdx.org/licenses/>).
- If you click the value of the License Name column, you can check detailed information for each license.

### Identifier
{: .specific-title} 
- The standardized short identifier makes it easier to identify the License and follows the SPDX notation (<https://spdx.org/licenses/>).

### License Type
{: .specific-title} 
- **Permissive**
    - Known as BSD-like or BSD-style License, these licenses have minimal requirements for software distribution.
    - Typically, it is required to maintain the copyright notice and disclaimer.
- **Weak Copyleft**
    - You can freely distribute copies and modified versions of the work on the condition that the same rights are retained in the derivative work. 
    - The source code of the original work and modifications must be disclosed.
- **Copyleft**
    - You can freely distribute copies and modified versions of the work on the condition that the same rights are retained in the derivative work. 
    - Not only the source code of the original work and its modifications but also the source code of any linked or integrated programs must be disclosed.
- **Proprietary**
    - Since it cannot be used without the permission of the software right holder, be sure to check the contractual relationship with respect to the use of the source code before using it.
- **Proprietary Free**
    - No additional contract is required, but can be used in specific terms and conditions or restrictions.

### Restriction
{: .specific-title} 
Restriction details were based on the [OSORI](https://osori-db.github.io/en/docs/guide/) project.
<style>
    .centered-table td:nth-child(3), .centered-table td:nth-child(4) {
        text-align: center;
    }
</style>

<table class="centered-table">
    <thead>
        <tr>
            <th scope="col">Restriction Type</th>
            <th scope="col">Description</th>
            <th scope="col">&nbsp;LEVEL&nbsp;</th>
            <th scope="col"><span style="white-space: nowrap;">Signal Light<br>(Restriction)</span></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td><strong class="highlight_table">Non-Commercial Use</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        Commercial use and distribution of software is prohibited. 
                        <br>
                        <span style="padding-left: 10px;">ex) CC-BY-NC-X.X</span>
                    </li>
                </ul>
            </td>
            <td>5</td>
            <td>🔴</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Internal Use Only</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        It allowed only for internal use.
                        <br>
                        <span style="padding-left: 20px;">ex) Additional-Buildcraft-Objects-Mod License</span>
                    </li>
                </ul>
            </td>
            <td>4</td>
            <td>🔴</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">No Charge</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        The license prohibits direct sales or charging of usage fees. (It can be embedded in free software provided by the company)
                        <br>
                        <span style="padding-left: 20px;">ex) Commons Clause License Condition v1.0, SIL Open Font License 1.1</span>
                    </li>
                </ul>
            </td>
            <td>3</td>
            <td>🟡</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">No Modification</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        You cannot distribute a modified version of the software. In other words, it should be used without modifying the source code.
                        <br>
                        <span style="padding-left: 20px;">ex) CC-BY-ND-X.X</span>
                    </li>
                </ul>
            </td>
            <td>2</td>
            <td>🟡</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">No Change the Name</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        This license does not allow to change name.
                        <br>
                        <span style="padding-left: 20px;">ex) IPA Font License</span>
                    </li>
                </ul>
            </td>
            <td>1</td>
            <td>🟢</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Platform Limitation</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        It is only available for use on specific platforms.
                        <br>
                        <span style="padding-left: 20px;">ex) Amazon Software License (must be used for web services, computing platforms, or applications provided by Amazon.com or its subsidiaries)</span>
                    </li>
                </ul>
            </td>
            <td>2</td>
            <td>🟡</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Purpose Restriction</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        Software cannot be used for a specific purpose(field).
                        <br>
                        <span style="padding-left: 20px;">ex) The Happy Bunny License (It cannot be used for military purposes)</span>
                    </li>
                </ul>
            </td>
            <td>2</td>
            <td>🟡</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Specification Restriction</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        The software must be used in accordance with specific specifications or standards.
                        <br>
                        <span style="padding-left: 20px;">ex) ETCPACK Software License Agreement (It can be used for compression and/or decompression according to the Khronos standard specifications)</span>
                    </li>
                </ul>
            </td>
            <td>2</td>
            <td>🟡</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Redistribution Restriction</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        Restricted software sub-components (Source Code, Binary file, etc.) that can be redistributed.
                        <br>
                        <span style="padding-left: 20px;">ex) SOFTWARE LICENSE FOR VIVANTE CORPORATION (TM) USER SPACE GRAPHICS DRIVER BINARY (It can only be redistributed in binary form)</span>
                    </li>
                </ul>
            </td>
            <td>5</td>
            <td>🟡</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Contract Required</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        It cannot be used without a commercial contract.
                        <br>
                        <span style="padding-left: 20px;">ex) QT Commercial License, NVIDIA Commercial License</span>
                    </li>
                </ul>
            </td>
            <td>5</td>
            <td>🔴</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Provide Installation Information Required</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        It must provide installation information.
                        <br>
                        <span style="padding-left: 20px;">ex) GPL-3.0</span>
                    </li>
                </ul>
            </td>
            <td>4</td>
            <td>🔴</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Patent Warning</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        This license may be subject to patent disputes and should be used with caution.
                        <br>
                        <span style="padding-left: 20px;">ex) Apple Public Source License</span>
                    </li>
                </ul>
            </td>
            <td>4</td>
            <td>🔴</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Network Triggered</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        Providing service over network is regarded as distribution, and the obligations of open source must be fulfilled.
                        <br>
                        <span style="padding-left: 20px;">ex) AGPL-3.0, OSL-2.0</span>
                    </li>
                </ul>
            </td>
            <td>3</td>
            <td>🟡</td>
        </tr>
        <tr>
            <td><strong class="highlight_table">Semi-Copyleft</strong></td>
            <td>
                <ul class="list-with-dot">
                    <li>
                        This license has restrictions, but there are no problems with use if the source code is disclosed.
                        <br>
                        <span style="padding-left: 20px;">ex) Ruby License</span>
                    </li>
                </ul>
            </td>
            <td>3</td>
            <td>🟡</td>
        </tr>
    </tbody>
</table>

### Source Code Disclosure Scope
{: .specific-title}
Select the scope of source code disclosure when distributing under each license. 
- **NONE** : No obligation to disclose
- **ORIGINAL** : Original open-source
- **FILE** : Source code disclosed on a file level
- **MODULE** : Source code disclosed on a module level
- **LIBRARY** : Source code disclosed on a library level
- **DERIVATIVE WORK** : The scope of legally defined derivative works
- **EXECUTABLE** : Source code disclosed for executable level
- **DATA** : The data itself
- **SOFTWARE USING THIS** : Any software that uses software under this license
- **UNSPECIFIED** : The source code must be disclosed, but the exact scope is unclear


### Obligation
{: .specific-title}
You can find out the notice and source code disclosure obligations for each license.
- **Notice**: If the checkmark (![ObligationCheck](images/check_icon.png)) is marked, it indicates an obligation to notify regarding copyright, license, or both.
- **Source**: If the checkmark (![ObligationCheck](images/check_icon.png)) is marked, it indicates an obligation to disclose the source code.

### Web site
{: .specific-title}
- Provides web site information of the original license. Click the URL to go to the site.

### User Guide
{: .specific-title}
- You can see the precautions when using the license.

## (Admin Only) Add, Modify, Delete License
{: .left-bar-title }
### Add
{: .specific-title}
![NEW_OSS](images/3_lic_add.PNG){: .styled-image width="80%"}
1. Click the Add button in the upper left of the License List.
2. At the "New_License" tab, enter the information of the new OSS.
    - **License Name** and **Nick Name** cannot be duplicated.
    - **Obligation** :
        - If Notice is checked, it is included in the OSS Notice.
        - If Source Code is checked, it is displayed as a list of source code collection OSS in the Packaging tab.
    - **User Guide** : Enter information about the OSS.
    - **Attribution** : When issuing an OSS Notice, enter the phrase that must be included separately.
3. Click the Save button(<img src="images/save_button.PNG" width="20" height="20" />) at the top right.

### Modify
{: .specific-title}
1. In the License List, click the License Name to be modified.
2. Make modifications on the License Details tab.
3. Click the Save button at the top right.

### Delete
{: .specific-title}
1. In the License List, click the license name you want to delete.
2. In the License Details tab, enter the reason for deletion in the Comment field.
3. Click the Delete button at the top right.
