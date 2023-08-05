# BaseStructure
BaseStructure is Project Framework

## Quick Start for Developer
1. Edit "paths.conf"
   1. Change PRJ_NAME and PRJ_ROOT for your project name and path.
   2. If you need more path, you can add here.
2. Edit "requirements.txt"
   1. Change library to latest version or you need.
   2. If you add more library, you must add here.


## Rules
1. Configure
   - Config files are set up separately for each library in the project.
     - Yaml
       - The .yml format is create for user editing.
       - Could write comments.
       - Don't insert multi yaml on one yaml file.
     - Json
       - The .js format is create for developer editing.
       - Can't write comments.
       - It is usually used to save data
     - Shell
     - 
       - The .conf format is create for launching from shell scripts.
       - Even after distribution, debug comments can be written and checked.
2. Data Export
   - Reduce unnecessary calculations
     - The data organized by information read from CSV, feature vectors, and data for visualization should be saved in Json format.
     - Most languages follow the Json format. 
     - Unifying the output in Json format is beneficial when using various models and for testing.
   - Visualization of results
     - Remember to change the output path if you want to visualize the results.
     - If you want to check temporarily, create a tmp folder outside the project and check it there.
     - If you want to check temporarily, create a tmp folder outside the project folder and check it there.

## File structure description
1. Examples
   - Place to shell scripts
2. Tests
   - It is used when there is something you want to try a little.
   - The role is the same as that of a research notebook.
   - .ipynb format file used with JupyterNotebook.
   - .ows format file used with Orange Data mining.
3. Logs
   - Please export any log file under this directory.