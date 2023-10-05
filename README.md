# Claire Lu & Dineth Meegoda - lab03-grammars

## 1. Wheat grammar puzzle
Iterations (n = 1, 2, 3) of the wheat one-rule grammar:\
<img width="200" alt="square1" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/bc486538-383f-44c5-b5c3-cecd33b9af3d">
<img width="200" alt="square2" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/1dd33b9a-f47c-431c-a9fb-ac8a70186edd">
<img width="200" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/11b4daaa-1b05-4f41-9c90-c9d5ff1021c6">

Rules:\
<img width="600" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/064bb722-0af0-4d14-8806-cd225baeea70">

## 2. Square grammar puzzle
Iterations (n = 1, 2, 3) of the square grammar:\
<img width="200" alt="square1" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/f2e93379-6fa8-4a91-ada2-d7f72b1363b1">
<img width="200" alt="square2" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/543fef50-dcce-48bc-b6b4-71229dbb49f9">
<img width="200" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/0d1b1d17-2bde-42a8-ab8d-70b4e1623580">

Rules:\
<img width="600" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/f52ba6f8-d85c-4033-b78f-000f13ded734">


## 3. Custom plant
For our custom plant, we wanted to make a nice round leaf that curved toward a point at the top!

Structure:
Our leaf is made of a series of straight and rotated lines. The needles that stick out from the spine are composed of rotated line segments, with each consecutive segment slightly more rotated, to form a line that looks like it's curving upwards. For symmetry, this is repeated on the other side of the spine. Then, this entire structure is repeated again as we travel up the spine of the leaf, each time becoming smaller.

This visual effect is achieved through our rules by making use of the iteration, i, and scaling the length of a line segment by some constant (less than 1) multiplied by i.

Iterations (n = 1, 2, 4, 10, 38) of our custom plant grammar:\
<img width="180" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/3a99f056-7855-4a35-851a-92abf130d499">
<img width="180" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/6806cb7a-c224-4ef3-bb72-35617f42de66">
<img width="180" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/ffb2d6ee-108c-4967-936d-1cea0dfa3842">
<img width="180" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/7c5f2301-1ad9-47b5-90d5-0c77e818848a">
<img width="180" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/a1ba6103-bd28-4027-82d7-508611366717">

Rules:\
<img width="600" alt="square3" src="https://github.com/ClaireL21/lab03-grammars/assets/102630261/846d0e29-76fb-4abf-b66a-90484d781865">
