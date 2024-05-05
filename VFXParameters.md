---
layout: default
title: VFX Parameters
nav_order: 3
---

### List Of VFX Graph Parameters

![image](https://github.com/SineVFX/CreativeLightsDoc/assets/37494885/965af473-5aa3-4687-aee1-133455bd39af)

### Heat Wave:
![image](https://github.com/SineVFX/CreativeLightsDoc/assets/37494885/15c34788-cec5-438e-b758-4e6c58da13e1)

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
* **Smoke Dissolve Edge Exp** - Higher values make the smoke dissolve more directional, similar to a gradient mask applied to a texture. Lower values make the dissolve more uniformly.
* **Heat Edge Noise** - Control the noise of Edge flame-like particles.
* **Flames Ramp Affected By OaD** - When being dissolved, controls how much the dissolve will affect the gradient ramp.
* **Flames Long Mask Exp** - Exp of a linear mask applied to flame particle sprites.
* **Depth Slope Step Size** - Parameters for Sobel-based edge detection in UV Space. Controls the thickness of edges, but higher values may produce unwanted artifacts.
* **Depth Hard Down Edge Distance** - Minimal Distance at which edge will be marked and particles will be spawned from it.
* **Edge Heat Move To Camera** - Move the Edge Heat Fill particles closer to the Camera, to remove some visual artifacts.
* **Dissolve Flame Enabled** - Enabled the Dissolve for the flames, providing a slightly different visual style.
* **Dissolve Flame Long Enabled** - Enabled the Dissolve for the flames, providing a slightly different visual style.
* **Soft Particles Distance Adjust Multiply** - Adjust the soft particles distance. If you notice that the particles are too soft when near opaque objects, try decreasing this setting.
 
Creative Light Script Component:
* **Resolution** - The Resolution of Depth Texture, use 512 for Heat Wave effects and any for Holo effects.
* **Projection** - Projection mode of the Camera.
* **Orthographic Size** - If using an Orthographic Camera, control its size.
* **Auto Scale Orthographic Size** - Scale the Orthographic Size parameter, based on the Lossy scale of the VFX.
* **Field Of View** - Controls the FoW parameter of the Perspective Camera.
* **Is Hologram** - Check if using any of Holo effects.
* **Dummy Cam** - Camera used for fake Depth Rendering.
* **Effect** - VFX Graph of the prefab.
* **Material** - Fake Depth material.

### Holo:
![image](https://github.com/SineVFX/CreativeLightsDoc/assets/37494885/28646075-63cb-49ac-8663-5e4e663d2e71)

VFX Graph:
* **MASTER** -  These parameters serve as a final layer of adjustments, multiplying parameters by the corresponding value.
* **Sequential Or Random Circle** - Switch between a scan-like effect or random spawn. This parameter is available only for Scan Holo VFX.
* **Glitch Enabled** - Enabled the subtle glitch-like effect.
* **Shape Circular** - Makes the shape of the effect circular, resembling a spotlight.
* **Shape Circular SS** - Parameters used for SmoothStep function.
* **Dots Mask** - Mask used for holo dots.
* **Clend Clamp Min** - Minimum Blend parameter, this will control the general speed of blending position of particles when moving the entire VFX.
* **Slope Length Multiply** - Multiply the slope length for each part of the VFX. This will control the Edge Detection style.
* **Light Range** - Range of the effect in World Units.
* **Light Range Exp** - Pow of the effect range, similar to light attenuation.
* **Opacity Slope Clamp Min and Max** - Min and Max parameters for Clamp function. This will alter the look of the Edge Detection part of VFX.
* **Spawn Rate** - Rate at which particles are being spawned.
* **Gradient Ramp Dots** - These parameters control the colorization of the effect.
* **Gradient Ramp Dots Adjust** - Multiply, Add, and Exp are used to control the gradient ramp mask. Imagine a 0 to 1 mask to generate a Ramp, you can add, multiply, or apply pow operators to it.
* **Gradient Ramp Dots Position** - Select a color for dots from the gradient ramp, 0 to 1 range.
* **Gradient Ramp Dots Use Slope** - Use slope from the Depth Map to colorize the dots.
* **Gradient Ramp Dots Slope Clamp Min and Max** - Clamp the slope by these parameters.
* **Emission Color** - Multiply the Ramp by Color.
* **Emission Intensity** - Controls the emission intensity of each element separately.
* **Scale Multiply** - Control the scale of VFX elements.
* **Depth Slope Step Size** - Parameters for Sobel-based edge detection in UV Space. Controls the thickness of edges, but higher values may produce unwanted artifacts.
* **Depth Slope Use Denominator** - Used an exact pixel distance for slope and edge detection.
* **Depth Hard Down Edge Enabled** - Mask the edges that are "in the shadow".
* **Depth Hard Down Edge Distance** - Minimal Distance at which edge will be marked and particles will be spawned from it.
* **Voxelize Position - Set of parameters** to discretize the position of dots particles.
* **Discretize UV** - Set of parameters to discretize the position of dots particles in UV space.
* **Cage Light Range Mode** - Mode in which cage rays will be multiplied by the color of dots using slope.
* **Cage Affected By Opacity Slope** - Cage rays now will pick a color from the gradient ramp based on slope.
* **Soft Particles Distance Adjust Multiply** - Adjust the soft particles distance. If you notice that the particles are too soft when near opaque objects, try decreasing this setting.
 
Creative Light Script Component:
* **Resolution** - The Resolution of Depth Texture, use 512 for Heat Wave effects and any for Holo effects.
* **Projection** - Projection mode of the Camera.
* **Orthographic Size** - If using an Orthographic Camera, control its size.
* **Auto Scale Orthographic Size** - Scale the Orthographic Size parameter, based on the Lossy scale of the VFX.
* **Field Of View** - Controls the FoW parameter of the Perspective Camera.
* **Is Hologram** - Check if using any of Holo effects.
* **Dummy Cam** - Camera used for fake Depth Rendering.
* **Effect** - VFX Graph of the prefab.
* **Material** - Fake Depth material.



### Support email: sinevfx@gmail.com
