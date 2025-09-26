# Day 3 - Combinational and sequential optmizations
## Introduction to optimizations

### Combinational op
- direct optimisation
- boolean logic reduction
#### Constant propagation 
It is a type of direct optimisation.

Example:

![alt text](image-14.png)

#### Boolean logic optimisaiton

![alt text](image-15.png)

### Sequential op

![alt text](image-16.png)

Sequential constant:

![alt text](image-17.png)

Cloning and retiming:

![alt text](image-18.png)

## Lab 1 - combinational Optimisations
### opt_check vs opt_check2
- opt_check - constant 0 propagation in a mux
- opt_check2 - constant 1 propagation in a mux
- opt_check3 - constant propagation in ternary mux eq `y=a?(c?b:0):0`
- opt_check4 - mux eq `y=a?(b?(a&c):c):(!c)`<br>
    <img src="image-23.png" alt="boolean reduction opt_check4" width="400"/>

- multiple_module_opt - constant propagation and unused pins in hierarchy<br>
    <img src="image-26.png" width="400"/>

- multiple_module_opt2 - instance pruning and constant propagation<br>
    <img src="image-27.png" width="400"/>

#### opt_check synthesis result:

![alt text](image-19.png)

#### opt_check2 synthesis result:

![alt text](image-20.png)

#### opt_check3 synthesis result:

![alt text](image-21.png)

#### opt_check4 synthesis result:

![alt text](image-22.png)

#### multiple_module_opt synthesis result:

![alt text](image-24.png)

#### multiple_module_opt2 synthesis result:

![alt text](image-25.png)

## Lab 2 - Sequential optimisations

### dff_const1 
simulation:<br>
<img src="image-28.png" width="600"/>
synthesis:<br>
<img src="image-31.png" width="600"/>

### dff_const2 
simulation:<br>
<img src="image-29.png" width="600"/>

synthesis:<br>
<img src="image-30.png" width="600"/>

### dff_const3 
simulation:<br>
<img src="image-32.png" width="600"/>

synthesis:<br>
<img src="image-33.png" width="600"/>

### dff_const4 
simulation:<br>
<img src="image-34.png" width="600"/>

synthesis:<br>
<img src="image-35.png" height="200"/>

### dff_const5 
simulation:<br>
<img src="image-36.png" width="600"/>


synthesis:<br>
<img src="image-37.png" height="200"/>

## unused outputs optimisation
This optimisation involves identifying and removing parts of a digital circuit's logic that do not contribute to its final function or output, thereby reducing circuit complexity, saving power, and minimizing the silicon area required for the design.