# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle

### Rule
premise: F

rule: F=FF-[FF]+FF-[FF]+FF-

angle: 28

![1696438409301](image/README/1696438409301.png)

Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

## 2. Square grammar puzzle
### Rule
premise: +F

rule: F=F+F-F-F+F

angle: 90

![1696433182966](image/README/1696433182966.png)


How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

## 3. Custom plant

premise: A
rule: 
1. A=+[FFFFFFFFFF-FFF-FFFFF----FFFFF-FFFFFFFFFF]-
2. B=+[FF-F-F-F-F--F-F-F-F-FF]----
3. C=+[FF-FF-FF-FF-FF---FF-FF-FF-FF-FF]----
4. F=FAB+B+B+C+
angle: 30

* Generation = 3
![1696437863862](image/README/1696437863862.png)
* Generation = 5
![Alt text](image.png)

I chose to draw a sunflower and take the image below as a reference. A sunflower can be broadly divided into two parts: the outer large petals and the inner circular section. I used A to draw the outermost petals, while B and C were used to create the inner shapes and details. A is responsible for drawing the finer petals since there are fewer of them, while B and C are used to draw thicker petals of different sizes. By stacking multiple angles of B and C, they form an approximation of a circular shape.

Source: [Sunflower](https://www.istockphoto.com/vector/sunflower-flower-isolated-gm927047528-254336166)

![1696437998749](image/README/1696437998749.png)

Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
