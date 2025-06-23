--- 
sort : 1
published: true
title: 2.Identification 
---


# Identification 
<div class="note">
Fill in the results of the Open Source Software analysis for the Project to release and receive a review from the OSPO.
</div>

{% include list.liquid all=true %}

## General Project's Identification Process
{: .left-bar-title }
- Fill in **3rd Party, DEP, SRC, BIN.** → Request a review by clicking the **Request** button in the BOM.  
        - [**3rd Party**](https://fosslight.org/hub-guide-en/tutorial/1_project/2_Identification/1_3rd_Party_Tab.html): Load 3rd party included in the project.  
        - [**DEP**](https://fosslight.org/hub-guide-en/tutorial/1_project/2_Identification/2_DEP_Tab.html): Upload the result of Dependency Analysis.  
        - [**SRC**](https://fosslight.org/hub-guide-en/tutorial/1_project/2_Identification/3_SRC_Tab.html): Upload the result of Source Code Analysis.  
        - [**BIN**](https://fosslight.org/hub-guide-en/tutorial/1_project/2_Identification/4_BIN_Tab.html): Upload the result of Binary Analysis.  
        - [**BOM**](https://fosslight.org/hub-guide-en/tutorial/1_project/2_Identification/5_BOM_Tab.html): Combine the OSS List written on the other tab and review the warning message and request a review.  

## (Enterprise Only) Identification Process for Platform-generated Project
{: .left-bar-title }
- BIN(Android), BIN(Yocto) Tab : Fill in each Tab → Request to review by clicking the Request button on each Tab.  
    - BIN(Android) : Upload the result of [Android Binary Analysis](https://fosslight.org/fosslight-guide-en/scanner/6_android.html).  
    - BIN(Yocto) : Upload the result of [Yocto Analysis](https://fosslight.org/fosslight-guide-en/scanner/5_yocto.html).  