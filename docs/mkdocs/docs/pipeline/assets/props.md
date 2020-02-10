# **Props**

A **Prop** is any asset that is **not** a **character**, such as a teapot, a knife, etc.

To simplify the pipeline, we consider the following points:
 
 * Variations of a same prop are stored in different files and are considered as a different prop.
 * Props **must** be considered as standalone elements that are ready to be located in a set.

***


## **Prop Working Files**

Following files are files that need to be generated from scratch by the different departments. They are the main
building blocks for a prop.

### **Prop Modeling File**

!!! info
    This file contains all the geometry for the prop. The geometry is stored following a specific hierarchy and 
    nomenclature. UVs are not stored in this file.

<center>

|  **Prop Modeling File**          |      |
| -------- |:------|
| **Department** | Modeling
| **File Extension** | **.ma**
| **File Name** | `[asset_name]`.ma
| **File Path** | Assets/Props/**[asset_name]**/**[version_folder]**/model

|  **Example - BookA**          |      |
| -------- |:------|
| **File Name** | BookA.ma
| **Working File Path** | Assets/Props/**`BookA`**/**`__working__`**/model
| **Published File Path** | Assets/Props/**`BookA`**/**`__model_v001__`**/model

</center>

***

### **Prop Shading File**

!!! info
    This file contains all the shading info (shaders and materials) used by the prop. Also contains paths to the textures
     used by the prop. In this file UVs of the geometry are created. Shaders have a specific nomenclature.

<center>

|  **Prop Shading File**          |      |
| -------- |:------|
| **Department** | Shading
| **File Extension** | **.ma**
| **File Name** | `[asset_name]`.ma
| **File Path** | Assets/Props/**[asset_name]**/**[version_folder]**/shading

|  **Example - BookA**          |      |
| -------- |:------|
| **File Name** | BookA.ma
| **Working File Path** | Assets/Props/**`BookA`**/**`__working__`**/shading
| **Published File Path** | Assets/Props/**`BookA`**/**`__shading_v001__`**/shading

</center>

***

### **Prop Textures Files**

!!! info
    Those files contains texture information used by the prop. Files should be stored in both .png format and also .tx, 
    which is the optimized file format used by Arnold renderer.

<center>

|  **Prop Textures Files**          |      |
| -------- |:------|
| **Department** | Shading
| **File Extension** | **.tx** **.png**
| **File Name** | `[asset_name]_[description]_[texture_type].[UDIM]`.tx
| **File Path** | Assets/Props/**[asset_name]**/**[version_folder]**/textures

|  **Example - HouseC_Glass_BaseColor.1014**          |      |
| -------- |:------|
| **File Name** | HouseC_Glass_BaseColor.1014.tx
| **Working File Path** | Assets/Props/**`HouseC`**/**`__working__`**/textures
| **Published File Path** | Assets/Props/**`HouseC`**/**`__textures_v001__`**/textures

</center>

***

### **Prop Layout Rig File**

!!! info
    This file contains the **layout** rigging setup of the prop. This rig is loaded by layout department and contains
    a simplified version of the rig. It uses prop proxy mesh.
    
    
<center>

|  **Prop Layout Rig File**          |      |
| -------- |:------|
| **Department** | Rigging
| **File Extension** | .ma
| **File Name** | [asset_name]_layout
| **File Path** | Assets/Props/**[asset_name]**/**[version_folder]**/rig/**[asset_name]_layout**.ma

|  **Example - BookA**          |      |
| -------- |:------|
| **File Name** | BookA.ma
| **Working File Path** | Assets/Props/**`BookA`**/**`__working__`**/rig
| **Published File Path** | Assets/Props/**`BookA`**/**`__rig_v001__`**/rig

</center>

***

### **Prop Animation Rig File**

!!! info
    This file contains the **animation** rigging setup of the prop. This is the rig used by animation department and contains
    all of necessary controls and setups to achieve the desired deformations by animators. This file must contains 
    hires model but also can contains a setup to switch between hires or proxy model.
    
    
<center>

|  **Prop Animation Rig File**          |      |
| -------- |:------|
| **Department** | Rigging
| **File Extension** | .ma
| **File Name** | [asset_name]_animation
| **File Path** | Assets/Props/**[asset_name]**/**[version_folder]**/rig/**[asset_name]_animation**.ma

|  **Example - BookA**          |      |
| -------- |:------|
| **File Name** | BookA.ma
| **Working File Path** | Assets/Props/**`BookA`**/**`__working__`**/rig
| **Published File Path** | Assets/Props/**`BookA`**/**`__rig_v001__`**/rig

</center>

***

## **Prop Exported Files**

Following files are files that are generated as a result of a publication. Those files are usually by different departments
in different steps of the pipeline.

**WIP**

***

## **Data Flow**

> Props Data Flow
![Props Data Flow](../../img/pipeline/props/dataflow.png?style=centerme)

***

## **Prop Publishing**

Once a prop is modeled and shaded, it must be validated and published, so prop data can continue travelling through the
pipeline.

### **Geometry**

!!! warning "IMPORTANT"
    The nomenclature and hierarchy of both Prop **Modeling** File and Prop **Shading** File **MUST** be the same one
    described in the following sections.

#### **Nomenclature**

!!! info
    All geometry nodes **MUST** follow this nomenclature:
    
    **`[description]_[side]_geo_[unique_id]`**
    
    All geometry group nodes **MUST** follow this nomenclature:
    
    **`[description]_[side]_grp_[unique_id]`**
    
    ***
    
    * **description**: This field gives a description of what that geometry node represents. It MUST use camelCase 
    nomenclature (for example: CoverLeatherStrap
    * **side**: This field defines the side in the prop the prop is located:
        * **m** or **c**: Middle/Center
        * **r**: Right
        * **l**: Left
    * **unique_id**: 4 digits unique identifier, by default it should be **0000**

The geometry stored in the **Prop Modeling File** **must** follow a specific hierarchy structure and nomenclature.

```
root
│
└───[geo_LOD]
│   │
│   └───geo
│       │
│       └───[description]_[side]_geo_[unique_id]
│       |
│       └───[description]_[side]_grp_[unique_id]
│             |
│             └───[description]_[side]_geo_[unique_id]
|             |
|             ...
...
```

!!! example "Example - BookA"

    ```
    root
    │
    └───high
    │   │
    │   └───geo
    │       │
    │       └───paperPages_c_geo_0000
    │       |
    │       └───cover_c_geo_0000
    │       |
    │       └───metalKnots_c_grp_0000
    │       |   |
    │       |   └───metalKnot_c_geo_0000
    |       |   |
    |       |   └───metalKnot_c_geo_0001
    │       |
    │       └───leatherStraps_c_geo_0000
    │           |
    │           └───leatherStrap_c_geo_0000
    |           |
    |           └───leatherStrap_c_geo_0001
    |            
    └───proxy
        │
        └───geo
            │
            └───proxy_c_geo_0000
    ```

> Prop Hierarchy and Nomenclature Example
![Props Hierarchy and Nomenclature](../../img/pipeline/props/props_example.png?style=centerme)

!!! warning
    In the above image, high model pivot point is located in (0, 0, 0) of the world and proxy has been translated to the right
    some units, this is only as an example, in a production asset both high and proxy pivot points and transformations **MUST**
    be located in the **center (0, 0, 0)** of the world.

***

#### **Pivot Points**

Pivot point of the **root group** of the hierarchy and **parent groups** for both **proxy** and **hires** models **MUST** 
be located in the **center (0, 0, 0)** of the world.

***

#### **Materials**

In order to properly store the shaders and to properly assign those shaders to proper geometry later in the pipeline we
must follow a proper nomenclature for materials and shaders.

**WIP**

***

#### **Model Validators**

Before publishing a model file, some validators/checkers are executed during publish process to make sure that the model
is ready to be send to the next department (without breaking the pipeline). The following validations are done:

**WIP**