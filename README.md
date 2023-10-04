# lab03-grammars

# Result

## 1. Wheat grammar puzzle

<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

### Rule
F=FF[-FF]F[-FF]FF-

![](1.png)

![](2.png)

![](3.png)


**Explain:** 

FF: This means the current line segment extends twice its length. The plant grows straight forward for two units.

[-FF]: This creates a branch. The plant turns left (due to -) and grows forward for two units (FF). Once the growth inside the branch is done (inside the [...]), the plant's state returns to where the branch started.

F: The plant continues growing straight forward for one unit.

[-FF]: Similar to the second step, this creates another branch. The plant again turns left and grows forward for two units.

FF-: The plant grows forward for two units, and then turns left.
## 2. Square grammar puzzle

<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

### Rule
F=F+F-F-F+F

![](4.png)

![](5.png)


**Explain:**

Move forward one unit (F)

Rotate 90 degrees to the right and move forward one unit (+F)

Rotate 90 degrees to the left and move one unit forward (-F)

Rotate 90 degrees to the left and move one unit forward (-F)

Rotate 90 degrees to the right and move forward one unit (+F)
## 3. Custom plant
**Fern Structure:**

A fern's structure can be broken down into a few key components:

Stem: The central part that provides support.
Fronds: The large divided leaves. These are the main visual components of the fern and they branch out from the stem. Each frond can have smaller sub-fronds, displaying a recursive pattern.

### Role
X

X -> F+[[X]-X]-F[-FX]+X

F -> FF

![](6.png)

**Explain:** 

Rule X: This rule mimics the growth of the fern. It starts by drawing the stem (F), then branching out ([...]) to create fronds and sub-fronds. The plus (+) and minus (-) symbols give it a twist and turn, capturing the natural randomness of ferns. Recursive usage of X in this rule ensures the fractal nature of ferns where each frond can have its own sub-fronds.

Rule F: This is a simple rule where every stem segment is elongated, simulating the growth of the stem.
