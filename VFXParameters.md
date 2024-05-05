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
* **Resolution** -
* **Projection** -
* **Orthographic Size** -
* **Auto Scale Orthographic Size** -
* **Field Of View** -
* **Is Hologram** -
* **Dummy Cam** -
* **Effect** -
* **Material** - 



### Support email: sinevfx@gmail.com
