# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

![image](https://github.com/kishayan02/lab03-grammars/assets/97934823/75bd4bd4-4b2e-477a-b2b3-242e60df1f72)


## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

![image](https://github.com/kishayan02/lab03-grammars/assets/97934823/e369ccea-db52-414f-b28f-94727f588700)


## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

The plant we chose was the flower called baby's breath (we did not get to the actual flower part, unfortunately)

![image](https://github.com/kishayan02/lab03-grammars/assets/97934823/0c21c3ef-6b0c-4a1a-80d2-fd872d613e67)


Here is our final product (with 4, 5, and 6 generations)

![image](https://github.com/kishayan02/lab03-grammars/assets/97934823/4323e4f3-0e10-4812-8dcc-1065bb628a46)
![image](https://github.com/kishayan02/lab03-grammars/assets/97934823/8a6c2b9d-e485-40e3-84dd-808c457c200b)
![image](https://github.com/kishayan02/lab03-grammars/assets/97934823/ba63f155-98d7-4550-83fb-def4ed09254a)

Here are our rules:

![image](https://github.com/kishayan02/lab03-grammars/assets/97934823/be8116dd-820e-468a-80b6-d9b8d77942e7)

Baby's breath has multiple branches that get shorter over time with flowers on the ends. Thus, we have two separate rules, one that separates the plant into 3 branches with probability 0.6 and the other that separates the plant into 2 branches with probability 0.4. Additionally, the branches become 0.7x shorter with every iteration. There is also a rotation angle of 25 to make sure the plant branches out sufficiently. 

