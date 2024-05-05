---
layout: default
title: About The Asset
nav_order: 1
---

## About the Asset

This VFX Asset consists of many prefabs with two distinct styles. The first style is some form of a heat energy wave, suited for fire-based effects. The second style is holographic, suited for the creation of sci-fi effects. Both effects use custom fake depth material, HDRP version uses Custom Passes on top of it. All effects are created with a Visual Effects Graph, and using an array of renderers to generate the Depth Map from them. You need to set all the meshes you want to be interactable in the editor or via script.

Asset using a total of four Visual Effects Graphs:

![image](https://github.com/SineVFX/CreativeLightsDoc/assets/37494885/441b5868-05c1-418b-b15b-ec95be6a49d5)

### Important Notes

* **(Engine)** Asset is using Visual Effects Graph, so it requires GPU Compute Shaders, however, Unity has plans to add CPU simulation

* **(HDRP)** VFX Prefabs for the HDRP version were built with Exposure set to 13.5. Change the Emission Power for darker scenes.

* **(HDRP, URP)** This VFX Asset looks much better in "Linear" Color Space, but if you using "Gamma" Color Space, you need to slightly decrease the Final Power (Emission Power) material parameter of each effect. You can check it in the "Edit > Project Settings > Player" TAB.
* **(HDRP, URP)** Image Effects are necessary in order to make a great-looking game, as well as our asset. Be sure to use "ACES Tone Mapping" and "Bloom".



### How To Use

* First of all, check the three scenes "DemoScene", "DemoSceneManualVFXSpawnExamples", and "DemoSceneUseCasesAndExamples" in the Scenes folder. The First one contains complete effect compositions. The second one contains an example of how you can call manual VFX Spawn functions for point and mesh Raycast systems. The third one contains various examples of how to use the effects.
* Read the corresponding docs page on each system to learn how to add the effects to your scene.



### Support email: sinevfx@gmail.com
