---
layout: default
title: VFX Parameters
nav_order: 3
---

### List Of VFX Graph Parameters

![image](https://github.com/SineVFX/CreativeLightsDoc/assets/37494885/965af473-5aa3-4687-aee1-133455bd39af)

### Heat Wave:

VFX Graph:
* **MASTER** -  These parameters serve as a final layer of adjustments, multiplying parameters by the corresponding value.
* **Light Range** - Range of the effect in World Units.
* **Light Range Exp** - Pow of the effect range, similar to light attenuation.
* **Spawn Rate** - Rate at which particles are being spawned.
* **Gradient Ramp** - These parameters control the colorization of the effect.
* **Gradient Ramp Adjust** - Multiply, Add, and Exp are used to control the gradient ramp mask. Imagine a 0 to 1 mask to generate a Ramp, you can add, multiply, or apply pow operators to it.
* **Emission Color** - Multiply the Ramp by Color.
* **Emission Intensity** - Controls the emission intensity of each element separately.
* **Sparks 01 Initial Expand** - Initial position expand of sparks when they are spawned.
* **Sparks 01 Velocity and Velocity Offset** - Controls the velocity of sparks.
* **Sparks 01 Color From Ramp** - Select a color for sparks from the gradient ramp, 0 to 1 range.
* **Sparks 01 Noise** - Controls the Noise used to add randomness to a particle's spawn, lifetime, and size. By increasing the Exp parameters, you can create a more "streamy" look, and vice versa.
* **Sparks 01 Turbilence** - Controls the Turbilence of Sparks.
* **Sparks Light Range Exp Adjust Multiply** - Control the Light Range Exp separately for the sparks. If you want the sparks to be at a more constant emission, use low Exp parameters for this.
* **Smoke Noise** - Control the noise parameters of smoke particles's texture.
* Smoke Dissolve Edge Exp - 
* Heat Edge - 
* Flames Ramp Affected By OaD -
* Flames Long Mask Exp -
* Depth Slope Step Size -
* Depth Hard Down Edge Distance -
* Edge Heat Move To Camera -
* Dissolve Flame Enabled -
* Dissolve Flame Long Enabled -
* Soft Particles Distance Adjust Multiply -
 
Strips:
* **Strips Texture** - Main texture for lightning strips.
* **Strips EoL** - Emission Over Lifetime.
* **Strips SAoL** - Size and Alpha Over Lifetime.
* **Strips UV Stretch and Center UV** - Stretching the UV, and the other parameter is used to center the lightning strips at the Start and the End points.
* **Strips To Center** - Using the "Center UV" helps texture to adjust the UV of the lightning strip, making it more visually pleasing.
* **Strips Noise** - Controls the Offset Noise that makes lightning look like lightning.
* **Strips Noise PoL** - Noise Power (Offset Intensity) over Lifetime.
* **Strips NPoL** - Noise Position over Lifetime.

Hit:
* **Hit Texture** - Main texture used for hit effects.
* **Hit SoL** - Size over Lifetime.
* **Hit EoL** - Emission over Lifetime.
* **Hit Move To Camera Fix** - Moves the hit quad sprite in the direction of a Camera. Useful to adjust the world geometry intersection of screen space quads.

Hi3 is a spherical explosion, I apologize for the inconsistent naming:
* **Hit3 SoL** - Size over Lifetime.
* **Hit3 OoL** - Opacity over Lifetime.
* **Hit3 EoL** - Emission over Lifetime.
* **Source** - Parameters to adjust the source Hit effects.

Main Strip:
* **Main Strip Lifetime and Hit Lifetime** - Lifetime in seconds of the Main Strip and Main Strip Hit effects.
* **Main Strip Profile** - Thickness profile of a lightning strip.
* **Main Strip Noise Mask Profile** - Profile that controls the amount of Offset Noise applied to a lightning strip.
* **Main Strip EoL** - Emission over Lifetime.
* **Main Strip AoL** - Alpha over Lifetime.
* **Main Strip B** - Parameters that control the overall shape and emission of the second and third Main Strips. The amount of Main Strips can be changed in a C# script, check the "Min and Max Numbers Of Main Strips" parameters.

Branched Strip:
* **Branched Lifetime and Hit Lifetime** - Lifetime in seconds of the Branched Strip and Branched Strip Hit effects.
* **Branched Profile** - Thickness profile of a lightning strip.
* **Branched EoL** - Emission over Lifetime.
* **Branched AoL** - Alpha over Lifetime.
* **Branched Start Min and Max** - Adjust the initial point from which the Branched Strip can be branched.
* **Branched Noise Blend** - Blends between Main and Branched Offset Noises, don't change too much.

Other Parameters:
* **Sparks2** - Various parameters to control the size and physical properties of Spark effects. Most parameter names are self-explanatory.
* **Transition** - Add a small touch to a lightning strip, making it appear more solid at the start and end points.
* **Disable Parameters** - These are used to disable some parts of VFX, that are not needed.
* **HIDDEN Parameters** - VFX Graph Won't allow hidden parameters to be changed from outside, so these are currently visible, don't change them.

### List Of C# Script Parameters

![s20](/assets/images/02.png)

* **Preview Gizmos In Editor** - Use this to preview Gizmos in the Editor to adjust the Max Distance.
* **Modes** - Two self-explanatory modes, Spherical and Cone.
* **Hemisphere Distance** - Exclude the possible Raycasts from a Spherical Shape.
* **Max Distance** - Maximum Raycast distance.
* **Max Distance Auto Scale Enabled** - Enabled the AutoScale based on the maximum distance, disable it if you want to scale the distance in real-time, but no the effect itself.
* **Max Distance Affected By Anchor** - Link the AutoScale to a Local Scale of a selected Transform.
* **Max Distance Anchor Multiply** - Multiply the Anchor AutoScale value.
* **Auto Scale Multiply** - Multiply the AutoScale value.
* **Cone Mode Circle Min Radius** - Minimum Radius of a frustum circle of a cone.
* **Cone Mode Circle Max Radius** - Maximum Radius of a frustum circle of a cone.
* **Maximum Number Of Attempts** - Control the number of failed Raycast attempts, use low value for better optimization.
* **Maximum Number Of Branched Attempts** - Control the number of failed Raycast attempts, use low value for better optimization.
* **Min Number Of Main Strips** - Set the min and max count of spawned Lightning Strips.
* **Man Number Of Main Strips** - Set the min and max count of spawned Lightning Strips.
* **Min Number Of Branched Strips** - Set the min and max count of spawned Lightning Strips.
* **Man Number Of Branched Strips** - Set the min and max count of spawned Lightning Strips.
* **Speed** - Speed in which the VFX and Raycast are triggered.
* **Speed Variation** - Speed variation curve, to make the VFX appear more natural.
* **Speed Variation Time** - Displayed Variation Time, useful for very dynamic Variation Time curves.
* **Speed Variation Time Speed** - Speed in which Time Variation is changing.
* **Random Branched Circle Min Radius** - Branched strips are triggered using Sphere Raycast, these parameters control min and max radius.
* **Random Branched Circle Max Radius** - Branched strips are triggered using Sphere Raycast, these parameters control min and max radius.



### Support email: sinevfx@gmail.com
