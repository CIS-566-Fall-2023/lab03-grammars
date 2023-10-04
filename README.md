# Kyra Clark and Linda Zhu's lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Premise: F

Rule 1: F = FF[+FF]F[+FF]FF+

![tree1_itr1](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/17ebcda9-42ed-49e8-91fc-3aee201caaa9)

![tree1_itr2](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/9b6fd328-b996-4e5e-998c-a336cb6643a4)

![tree1_itr3](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/8d8e9751-adf7-4b1a-9d5c-ec34b10558fa)



Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

## 2. Square grammar puzzle
Premise: +F

Rule 1: F=F+F-F-F+F

![tree2_itr1](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/8b515c51-dfa5-411a-892e-a888704e16b6)

![tree2_itr2](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/810c5d08-453d-4f6a-bcb5-c99d07eb0a57)

![tree2_itr3](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/22dec898-0fc0-46cb-bfc6-fd6723efdd19)

Some extra fun: iteration = 4!

![tree2_itr4](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/74e081b8-b026-4acf-b18f-ce78d2ea7495)


How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

## 3. Custom plant
We want to make a dandelion using L-systems. Below are the results in 2D and 3D.

2D: We want to step upward and expand both sides by rotating +/- some degrees. Once the iterations increase, we also want to decrease the step size and the angle size.

![tree3](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/1769d376-2653-4d18-b031-164b6fcfda27)

3D is just to rotate the 2D patterns around y-axis.

![tree3_3d](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/af1d0a00-6900-4ff3-93bd-c5ade793e75f)

Next we did some tweaking of the parameters such as angle, angle scale, step size scale, etc.

![customFern](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/0fb319c2-16ad-4905-8bb2-5ce618b24b8b)

![customDandelion3D-2](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/b0c3f79c-70e8-42a4-a267-90af165f8be7)

![customDandelion3D](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/cd9334ad-c93c-4c88-9cb6-dc57495f78dc)

Below are the reference images we used.
![l-system-dandelion](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/4c469014-acb8-48fc-8965-ef0a959d1010)

![real-dandelion](https://github.com/LinDadaism/ProceduralGraphics-lab03-grammars/assets/46789205/9eb9c759-e74b-4b61-a4f9-0ce687f52e35)


Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
