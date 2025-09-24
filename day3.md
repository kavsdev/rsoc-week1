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

## Optimisations lab 1
### opt_check vs opt_check2
- opt_check - constant 0 propagation in a mux
- opt_check2 - constant 1 propagation in a mux
- opt_check3 - constant propagation in ternary mux eq `y=a?(c?b:0):0`
- opt_check4 - mux eq `y=a?(b?(a&c):c):(!c)`

    <img src="image-23.png" alt="boolean reduction opt_check4" width="400"/>

- multiple_module_opt - constant propagation and unused pins in hierarchy
    <img src="image-26.png" width="400"/>

- multiple_module_opt2 - instance pruning and constant propagation
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
