---
sort: 1
published: true
---

# Derivative Model Project

When conducting the OSC Process for a derivative model that uses software similar to an existing model, 
you can carry out more efficiently by [copying the completed project](../2_project/3_reuse_project/1_copy_project.md) 
of the previous model.

## If a few open sources are additionally used in the base model
- When copying the project, select **Identification Progress** to copy the open source list of the base model project as it is.
- Enter the information of the additional open sources in the Identification tab.

## If the new project version uses the same OSS as the existing project
- Use [BOM Compare](../2_project/2_using_project_info/1_bom_compare.md) to check if the final OSS list is the same.
- If the OSS usage and the source code to be disclosed are the same:
  - You can substitute the OSC Process by using the OSS notice issued for the existing project.
- If the OSS usage is the same but the source code to be disclosed is different:
  - This applies to minor changes such as modifying the README file or Notice file of the OSS Package.
  - When [copying the project](../2_project/3_reuse_project/1_copy_project.md), 
    select the **Packaging Confirm** stage.
  - After [changing the OSS package file in the Distribution tab](../2_project/5_distribution/2_modify_oss_package.md),
    proceed with the distribution.

