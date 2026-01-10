## Original Problem

Importing 3D models and assets is an important part of 3D modeling and BIM workflows, and that is why it is important that the model selection, preview and importing is a seamless process that does not interfere and slow down modeling.

That is the main problem of the current FreeCAD 3D model library. Most of the library models do not have image previews, and users do not know what models they are importing.

Another issue is that the quality of the previews which are currently availabe is of low resolution and they are barely visible.

Some other issues are not critical but could use improvement, such as exposing the new link option to users direcly from the model library.

## Key Enhancements In This Fork

### 3D Model Library Preview System
Improved 2D and 3D preview capabilities in the [FreeCAD BIM Workbench](https://github.com/yorikvanhavre/BIM_Workbench) model library browser, and added new buttons for inserting and adding models.

**Features:**
- High-res 2D thumbnail generation for quick visual browsing of selected models
- Previews are generated for every library item
- Optional 3D model preview for each selected model
- Added new buttons for inserting and adding models

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5bb400ad-2d98-4e55-a518-8fdabd59cfa6" />

**Implementation:**
- Utilizes save file option to generate new images in a 512x512 resolution
- Reference the generated images and use them as a preview for each selected file
- Added buttons and fixed image preview display in Qt designer
- Connected buttons in Python
