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
![Image](https://github.com/yuhanliu-tech/lab03-grammars/blob/main/l-systems-slug2.png)

We have two main components: the slug's body and the slug's frilly limbs. 
Thus, we assigned a rule to generate each: X for the body and Z for the frilly limbs. 
We also chose to keep the angle and iteration length small so that we could compound F and +/- as to increase the angle or step sizes. 

The X rule breaks down the slug's body into parts. First, we added few F steps to create the long tail, before moving into the first pair of frilly limbs. We noticed that the angle of the frilly limbs moves closer to 90 degrees as the limbs become bigger. Thus, we used the + and - operators to account for this in creating the second and third limb pairs. We also slowly add in angle changes to create the arc in the slug body. Finally, we created the Y-shaped head using more Fs. The X rule calls the Z rule when creating the frilly limb.

The Z rule creates fans on top of itself to form the slug's frilly limbs. We also made it recursive, so that the limbs round out and have more frills as the iteration increases, but we found iteration 2 to be most accurate (an image of a higher iteration is included for fun, it has some pretty crazy frills but keeps the overall slug shape). In short, we focused on creating an accurate representation of the slug shape (even though it's a line drawing) over complexity of the l-system. 

If we have more time, we'd like to port the rules into Houdini's l-system. Then, we could form the actual sea slug by copying a teardrop mesh shape to all the curves of the slug. We could even animate the slug by adjusting the angle parameter in the l-system. 

![Image](https://github.com/yuhanliu-tech/lab03-grammars/blob/main/l-systems-slug.png)
