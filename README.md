# lab03-grammars
Diana Ouyang and Yuhan Liu practiced grammars. 
Special thanks to this awesome [L-Systems Renderer](https://piratefsh.github.io/p5js-art/public/lsystems/). 

## 1. Wheat grammar puzzle
![Image](https://github.com/yuhanliu-tech/lab03-grammars/blob/main/l-systems1.png)

## 2. Square grammar puzzle
![Image](https://github.com/yuhanliu-tech/lab03-grammars/blob/main/l-systems.png)

## 3. Blue Sea Dragon
For our custom L-system, we decided to try and replicate a cute blue sea slug. 

![Image](https://github.com/yuhanliu-tech/lab03-grammars/blob/main/blueseadragon.jpg)

Our final L-System Render is here. 
![Image](https://github.com/yuhanliu-tech/lab03-grammars/blob/main/l-systems2.png)

We have two main components: the slug's body and the slug's frilly limbs. 
Thus, we assigned a rule to generate each: X for the body and Z for the frilly limbs. 
We also chose to keep the angle and iteration length small so that we could compound F and +/- as to increase the angle or step sizes. 

The X rule breaks down the slug's body into parts. First, we added few F steps to create the long tail, before moving into the first pair of frilly limbs. We noticed that the angle of the frilly limbs moves closer to 90 degrees as the limbs become bigger. Thus, we used the + and - operators to account for this in creating the second and third limb pairs. Finally, we created the Y-shaped head using more Fs. The X rule calls the Z rule when creating the frilly limb.

EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 
