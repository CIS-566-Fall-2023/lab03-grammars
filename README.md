# L-Systems : Utkarsh Dwivedi & Saksham Nagpal

## 1. Wheat Grammar
```
Premise: F
Rule: F=FF[-FF]F[-FF]FF-
Angle: 20
```

![](images/g1.png)

| ![](images/g11.png) | ![](images/g2.png) | ![](images/g3.png) |
|:--:|:--:|:--:|
| *iterations=1* | *iterations=2* | *iterations=3* |

## 2. Square Grammar
```
Premise: +F-
Rule: F=F+F-F-F+F
Angle: 90
```

| ![](images/g22.png) | ![](images/g23.png) | ![](images/g34.png) | ![](images/g45.png) |
|:--:|:--:|:--:|:--:|
| *iterations=1* | *iterations=2* | *iterations=3* | *iterations=4* |

## 3. Custom L-System
We wanted to make a snowflake for our custom L-system, so we tried a bunch of stuff and this is what we finally came up with. This is the grammar that we used:
```
Premise:        D
Rule1:          C=F[--F(.2)C][++F(.2)C]FC[--F(.13)C][++F(.13)C]FC[--FC][++FC]FC
Rule2:          D=[C]+(60)[C]+(60)[C]+(60)[C]+(60)[C]+(60)[C]
```

| ![](images/ref.png) |
|:--:|
| *Reference image (not really)* |

![](images/snowflake1.jpg)

![](images/demo.gif)

| ![](images/sfiter1.jpg) | ![](images/sfiter2.jpg) | ![](images/sfiter3.jpg) | ![](images/sfiter4.jpg) |
|:--:|:--:|:--:|:--:|
| *iterations=1* | *iterations=2* | *iterations=3* | *iterations=4* |

