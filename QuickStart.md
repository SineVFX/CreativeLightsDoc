---
layout: default
title: Quick Start
nav_order: 2
---

## Quick Start

* Drag And Drop VFX Prefab from the "Assets\SineVFX\CreativeLights\CompleteEffectsPrefabs" folder into your scene.
* Position the Effect as you see fit, the included Spot Light will help you with this.
* Select the prefab parent game object with a "CreativeLight" component.
* Add all the renderers into a "Renderers" array. Depth Texture will use these objects for rendering.
* There is an included "DummySphereForDepth" renderer, do not remove it.
* Select the child game object with VFX Graph and adjust the "MASTER Scale" and "Light Range" parameters as you see fit.
* ![image](https://github.com/SineVFX/CreativeLightsDoc/assets/37494885/d2cb805b-1738-4cb1-b1f2-74f5d42cda4d)
* After that the effect should work properly, for further customization, check the "VFX Parameters" page.
* HDRP Only: If you want to update the renderers during gameplay, check the "Update Custom Pass Materials" bool or call the "UpdateCustomPassParameters()" function.

The parameters can be changed in the "Creative Light" script component and the VFX Graph. The "Creative Light" script component controls Resolution, Camera Perspective mode, and Field Of View. The VFX Graph parameters control the visual looks of the effect.

### Common Adjustments

* **(Scale)** To scale the effect after dropping it into your scene you can adjust two parameters, "MASTER Scale" and "Light Range". The effect elements will be scaled with the "MASTER Scale", and how far the effect will go with the "Light Range" parameter.
* **(Color)** Color can be changed in the Visual Effects Graph parameters. Gradient Ramps are used to colorize the effects, the easiest way to tweak the color is to change these textures. You can also adjust the "Emission Color" parameters for more subtle tweaks.
* **(Speed)** "Spawn Rate" parameters will affect the spawn speed of particles. If you can see that the particle spawn is inconsistent or choppy, open the corresponding VFX Graph and increase the Capacity.
* ![image](https://github.com/SineVFX/CreativeLightsDoc/assets/37494885/64af075e-2f9e-430d-9c37-5606bfc89837)



### Support email: sinevfx@gmail.com
