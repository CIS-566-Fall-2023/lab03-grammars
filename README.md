# Kyra Clark and Linda Zhu's L-system Lab
Let's practice using grammars! For this lab, we used the L-system node in Houdini.

## 1. Wheat grammar puzzle
Premise: `F`

Rule 1: `F = FF[+FF]F[+FF]FF+`

![tree1_itr1](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/17ebcda9-42ed-49e8-91fc-3aee201caaa9)

*Figure 1: wheat grammar iteration = 1*

![tree1_itr2](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/9b6fd328-b996-4e5e-998c-a336cb6643a4)

*Figure 2: wheat grammar iteration = 2*

![tree1_itr3](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/8d8e9751-adf7-4b1a-9d5c-ec34b10558fa)

*Figure 3: wheat grammar iteration = 3*

## 2. Square grammar puzzle
Premise: `+F`

Rule 1: `F = F+F-F-F+F`

![tree2_itr1](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/8b515c51-dfa5-411a-892e-a888704e16b6)
*Figure 4: square puzzle iteration = 1*

![tree2_itr2](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/810c5d08-453d-4f6a-bcb5-c99d07eb0a57)
*Figure 5: square puzzle iteration = 2*

![tree2_itr3](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/22dec898-0fc0-46cb-bfc6-fd6723efdd19)
*Figure 6: square puzzle iteration = 3*

Some extra fun: iteration = 4!

![tree2_itr4](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/74e081b8-b026-4acf-b18f-ce78d2ea7495)

## 3. Custom plant
We wanted to make a dandelion based on the reference images below.

![real-dandelion](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/9eb9c759-e74b-4b61-a4f9-0ce687f52e35)

We found this possible L-system example that looked like the kind of shape we wanted, where a root-shoot axis produces leaves that extend outward. Next, we tried to match this structure.

![l-system-dandelion](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/4c469014-acb8-48fc-8965-ef0a959d1010)

We started in 2D to create a possible cross-section of our dandelion. We wanted to step upward and expand both sides by rotating +/- some degrees. Once the iterations increase, we also want to decrease the step size and the rotation so that the stems grow shorter at the tip of the crown with leaves occurring in a circular pattern. 

![tree3](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/1769d376-2653-4d18-b031-164b6fcfda27)
*Figure 7: Rules for 2D base shape*

![customDandelion2D](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/5988426b-e688-40b1-b8d6-8038c1092353)

*Figure 8: Fine tunning values to achieve a desired result at iteration = 13, which takes ~40 min for Houdini to compute.*


Our first attempt at 3D was to just rotate the 2D patterns around y-axis.

![tree3_3d](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/af1d0a00-6900-4ff3-93bd-c5ade793e75f)
*Figure 9: Adding multiple counter-clockwise rolls to the base rule creates a 3D tree.*

Next we did some tweaking of the parameters such as rotation angle, angle scale, step size scale, etc, until we got a pattern we were satified with. 

![customFern](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/0fb319c2-16ad-4905-8bb2-5ce618b24b8b)

*Figure 10: When experimenting with the grammar, we found stacking up two replica produces a structure that looks like ferns. Surprise!*

![customDandelion3D](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/cd9334ad-c93c-4c88-9cb6-dc57495f78dc)

*Figure 11: Back to our dandelion, instead of adding multiple default roll command which uses the same angle as the branches in 2D, we replaced it with a single roll of a custom angle, b, so the crown looks more organic.*

### Final L-System Dandelion: 
![customDandelion3D-2](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/b0c3f79c-70e8-42a4-a267-90af165f8be7)
