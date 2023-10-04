## Name
Chang Liu & Tianyi Xiao

## Rules & Images
### 1. Wheat grammar puzzle
#### rules
`F=FF[+FF]F[+FF]FF+`

(angle = 20 degrees)
#### iteration = 3
![](lsystem_1.png)
#### iteraton = 4
![](lsystem_1_4.png)

### 2. Square grammar puzzle
#### rules
`F=F-F+F+F-F`

(angle = 90 degrees)

![](lsystem_2_rules.png)
#### iteration = 3
![](lsystem_2.png)
#### iteraton = 4
![](lsystem_2_4.png)

### 3. Custom Plant
#### rules
Premise: `AF`

Rule 1: `A = [\+F[\+F]/-F][/-F[/-F][\+F]]`

Rule 2: `F = FAF`

![](lsystem_3_rules.png)
#### designs explain
For our L-System grammar, first of all, I design the first rule to make the branch of our tree grow into two sub-branch in symmetry directions, and then each has its own sub-sub-branches.
Then, the second rule makes sure that the whole tree can grow into left, right, and straight directions, with different scales.

### results
![](lsystem_3.png)

# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
