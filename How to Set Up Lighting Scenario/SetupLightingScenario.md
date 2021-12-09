# How to Set Up Lighting Scenarios Using the Variant Manager

This document will take you step-by-step through the tasks required to set up a lighting scenario using the variant manager in Unreal Engine 4.

Using the variant manager can be an alternative way to create lighting scenarios from the standard method.

The benefits of using the variant manager are:
* iterate many lighting scenarios on one level.
* give team members a simple to use setup.
* create a more organized file structure.


## Prerequisite

To use the Variant Manager, you need to have the **Editor > Variant Manager** plugin enabled for your project.

You need to be familiar with the basics of Lighting Scenarios and the Variant Manager.
If not, follow these links to learn more:  
[Precomputed Lighting Scenarios](https://docs.unrealengine.com/4.27/en-US/BuildingWorlds/LightingAndShadows/PrecomputedLightingScenarios/)  
[Variant Manager Overview](https://docs.unrealengine.com/4.27/en-US/WorkingWithContent/Variants/Overview/)

## Set Up the Lighting Scenario Scene

1. Create a **New Level** using the **TimeOfDay** Template.

![LS01_TimeofDayTemplate](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/LS01_TimeofDayTemplate.png)

<br/>

2. In the World Outliner, delete the **Floor, PlayerStart, SM_MatPreviewMesh_01, TextRenderActor**, and **TextRenderActor2** actors.

![LS02_DeleteActors](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/LS02_DeleteActors.png)

<br/>

3. In the Content Browser, right click and select **Miscellaneous > Level Variant Sets.**

![LS03_CreateLVS](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/LS03_CreateLVS.png)

<br/>

4. Select the **Level Variant Sets**. Right click > **Rename** and change to *LightingScenario01*.

![LS04_RenameLVS](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/LS04_RenameLVS.png)

<br/>

5. Open *LightingScenario01* to pop up the **VariantManager** Window.

![LS05_VMPopUp](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/LS05_VMPopUp.png)

## Set Up the Variant Manager

1. In the VariantManager window, click **+Variant Set.**

![VM01_CreateVSet](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/VM01_CreateVSet.png)

<br/>

2. Click the **+ symbol** next to the created Variant Set.

![VM02_CreateVariant](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/VM02_CreateVariant.png)

<br/>

3. Rename the Variant to *Day.*

![VM03_RenameDay](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/VM03_RenameDay.png)

<br/>

4. In the Properties tab, click the **Actors+ -> DirectionalLight.**

![VM04_AddDLight](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/VM04_AddDLight.png)

<br/>

5. Repeat the step to **add the rest of the actors.**

![VM05_AddAll](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/VM05_AddAll.png)

<br/>

6. On the *Day* Variant, right click > **Duplicate** to create another variant.

![VM06_DuplicateDay](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/VM06_DuplicateDay.png)

<br/>

7. Rename the new Variant to *Sunset.*

![VM07_RenameSunset](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/VM07_RenameSunset.png)

## Configure Your Lighting Scenario Variants

1. In the Day Variant, select the **DirectionalLight.**

![ConLSV01_SelectDLight](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLSV01_SelectDLight.png)

<br/>

2. Click the **record symbol** at the top of the VariantManager window to enable auto-capture properties.

![ConLSV02_RecordDay](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLSV02_RecordDay.png)

<br/>

3. In the Details window, change the **Y-Axis Rotation** to **-50.**

![ConLSV03_Rotation50](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLSV03_Rotation50.png)


<br/>

4. In the *Sunset* Variant, select the **DirectionalLight.**

![ConLSV05_SelectSunset](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLSV05_SelectSunset.png)

<br/>

5. Change the **Y-Axis Rotation** to **-2.**

![ConLSV07_Rotation02](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLSV07_Rotation02.png)

<br/>

6. Click the **record symbol** to disable auto-capture properties.

![ConLSV08_DisableSunset](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLSV08_DisableSunset.png)

<br/>

7. In the Content Browser, select *LightingScenario01* and right click > **Save.**

![ConLSV09_SaveLSFile](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLSV09_SaveLSFile.png)

<br/>

Select the variants to toggle between the Day and Sunset lighting scenarios.

![ConLVS10_CompareLS](https://raw.githubusercontent.com/alanm01/LightingScenarios/main/How%20to%20Set%20Up%20Lighting%20Scenario/Images/ConLVS10_CompareLS.png)

## Next Steps
This guide shows an example of changing a single property on the DirectionalLight. Repeat the process for other properties and actors to get your desired lighting.

Follow the [Precomputed Lighting Scenarios](https://docs.unrealengine.com/4.27/en-US/BuildingWorlds/LightingAndShadows/PrecomputedLightingScenarios/) guide to import the level into your project.

Learn more about lighting settings on the [Unreal Engine Documentation](https://docs.unrealengine.com/4.27/en-US/BuildingWorlds/LightingAndShadows/) site.
