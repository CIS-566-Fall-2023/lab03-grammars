# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

### Screenshots of iterations and rules 
<img width="600" alt="square1" src="wheat-grammar-n=1.png">
<img width="600" alt="square2" src="wheat-grammar-n=2.png">
<img width="600" alt="square3" src="wheat-grammar-n=3.png">
<img width="600" alt="square4" src="wheat-grammar-rules.png">

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

NOTE: adjusted angle to 20


### Screenshots of iterations and rules 
<img width="600" alt="square1" src="square-grammar-n=1.png">
<img width="600" alt="square2" src="square-grammar-n=2.png">
<img width="600" alt="square3" src="square-grammar-n=3.png">
<img width="600" alt="square4" src="square-grammar-rules.png">

NOTE: adjusted angle to 90  

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

### Screenshots of iterations and rules 
<img width="600" alt="square1" src="cordate-leaf-n=3.png">
<img width="600" alt="square2" src="cordate-leaf-n=6.png">
<img width="600" alt="square3" src="cordate-leaf-n=12.png">
<img width="600" alt="square4" src="cordate-leaf-rules.png">

For my custom plant, I chose to replicate a cordate leaf (aka a heart shape leaf). \
I drew polygon surfaces with my L-systems using the following commands: \
{ = Start a polygon \
. = Make a polygon vertex \
} = End a polygon 

My rules were as follows: \
A=[+A{.].C.} \
B=[-B{.].C.} \
C=FFFC 
- A and B are called to rotate/branch off in two different directions (one counterclockwise and the other clockwise) to draw two mirroed sections of the leaf. They are what handle the rotation/branching and drawing of the polygon surfaces. C handles the length of the leaf segment. With the addition of C to A and B, we are able to form longer leaf segments with wider angles with every generation, thereby creating a heart-shape for the leaf instead of just a circular shape. 


## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
