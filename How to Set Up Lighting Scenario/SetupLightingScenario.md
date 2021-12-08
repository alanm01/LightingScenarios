# How to Set Up Lighting Scenarios Using the Variant Manager

This document will take you step-by-step through the tasks required to set up a lighting scenario using the variant manager in Unreal Engine 4.

Using the variant manager is an alternative way to create lighting scenarios from the standard method.

The benefits of using the variant manager are:
* to speed up the iteration process.
* give better usability to team members.
* create a more organized file structure.


## Prerequisite

To use the Variant Manager, you need to have the **Editor > Variant Manager** plugin enabled for your project.

You need to be familiar with the basics of Lighting Scenarios and the Variant Manager.
If not, follow these links to learn more:
[Precomputed Lighting Scenarios](https://docs.unrealengine.com/4.27/en-US/BuildingWorlds/LightingAndShadows/PrecomputedLightingScenarios/)
[Variant Manager Overview](https://docs.unrealengine.com/4.27/en-US/WorkingWithContent/Variants/Overview/)

## Set Up the Lighting Scenario Scene

1. Create a New Level using the TimeOfDay Template.

![Step 01](https://raw.githubusercontent.com/alanm01/Tech-Writing-Workshop/main/Github%20Profile/Github%20Profile%20-%20Step%2001.png)

2. In the World Outliner, delete the Floor, PlayerStart, SM_MatPreviewMesh_01, TextRenderActor, and TextRenderActor2 actors.

3. In the Content Browser, right click and select Miscellaneous -> Level Variant Sets.

4. Right click > Rename and change to LightingScenario01.

5. Double click LightingScenario01 to pop up the VariantManager Window.

## Set Up the Variant Manager

1. In the VariantManager window, click +Variant Set.

2. Click the + symbol next to the created Variant Set.

3. Rename the Variant to Day.

4. In the Properties tab, click the Actors+ -> DirectionalLight.

5. Repeat the step to add the rest of the actors.

6. On the Day Variant, right click > Duplicate to create another variant.

7. Rename the new Variant to Sunset.

## Configure Your Lighting Scenario Variants

1. In the Day Variant, select the DirectionalLight.

2. Click the record symbol at the top of the VariantManager window to enable auto-capture properties.

3. In the Details window, change the Y-Axis Rotation to -50.

4. Click the record symbol to disable auto-capture properties.

5. In the Sunset Variant, select the DirectionalLight.

6. Click the record symbol.

7. Change the Y-Axis Rotation to -2.

8. Click the record symbol to disable.

9. In the Content Browser, select LightingScenario01 and right click > Save.


Double click the variants to toggle between the Day and Sunset lighting scenarios.

## Next Steps
This guide shows an example of changing a single property on the DirectionalLight. Repeat the process for other properties and actors to get your desired lighting.

Learn more about lighting settings on the [Unreal Engine Documentation](https://docs.unrealengine.com/4.27/en-US/BuildingWorlds/LightingAndShadows/) site.