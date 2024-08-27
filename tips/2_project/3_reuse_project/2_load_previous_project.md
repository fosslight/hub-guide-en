---
sort: 2
published: true
---

# Importing Analysis Results from Other Projects

You can import previously analyzed project results and apply them to a new project. 
This feature is useful in the following scenarios:

1. When a project is divided into multiple modules, and each module's open source analysis is performed separately, 
   then combined for management.
2. When there are multiple projects utilizing common modules.

- How to Import Previous Project Analysis Results:
<br/>
You can load each results in the 3rd party, SRC, DEP, and BIN tabs of the Identification stage.
<br/>
Note: Only projects with the **Identification stage completed** can be imported.

1. Click the tab where you want to load the analysis results.
2. Click the Project Search button.
   ![ProjectSearch](../../images/project/load_project/project_search.png){: width="80%"}
    - If you are in View mode, click the Edit button (![EditBtn](../../images/project/load_project/edit-solid.png){: width="1.5%"}) 
      to see the Project Search button.
3. Choose your search criteria and enter the desired search term.
   ![ProjectSearchBar](../../images/project/load_project/project_search_searchbar.png){: width="80%"}
4. Select the project you want to import from the search results.
   ![ProjectSearchResult](../../images/project/load_project/project_search_result.png){: width="80%"}
5. The Detail Preview menu will appear below the search list, showing the list of open source components to be loaded.
   Click the Load button.
   ![ProjectSearchDetailPreview](../../images/project/load_project/project_search_detail_preview.png){: width="80%"}
6. Choose the desired import method in the popup.
   ![ProjectLoadPopup](../../images/project/load_project/project_load_popup.png){: width="80%"}
    - Reset & Load: Clears the existing contents in the OSS table and loads the open source list from the selected project.
    - Load & Append: Keeps the existing contents in the OSS table and adds the open source list from the selected project.