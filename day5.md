# Day 5 - Optimization in synthesis
## `if`, `case` constructs
Priority logic:
<br><img src="image-52.png" width="400"/><br>


Inferred latch -  incomplete else in if
<br><img src="image-54.png" width="400"/><br>
<br><img src="image-60.png" width="400"/><br>

Case:
<br><img src="image-55.png" width="400"/><br>
<br><img src="image-56.png" width="400"/><br>
<br><img src="image-57.png" width="400"/><br>
<br><img src="image-58.png" width="400"/><br>

## Lab - `if`
### incomp_if:
Simulation:
<br>![alt text](image-61.png)<br>
Synthesis:
<br>![alt text](image-62.png)<br>

### incomp_if2:
Simulation:
<br>![alt text](image-63.png)<br>
Synthesis:
<br>![alt text](image-64.png)<br>

## Lab - `case`
### incomp_case :
Simulation:
<br>![alt text](image-65.png)<br>
Synthesis:
<br>![alt text](image-66.png)<br>
### comp_case:
Simulation:
<br>![alt text](image-67.png)<br>
Synthesis:
<br>![alt text](image-68.png)<br>
### partial_case_assign:
Simulation:
<br>![alt text](image-69.png)<br>
Synthesis:
<br>![alt text](image-70.png)<br>

### bad_case:
Simulation and GLS:
<br>![alt text](image-72.png)<br>
Synthesis:
<br>![alt text](image-71.png)<br>

## For Loop and For Generate
![alt text](image-73.png)

![alt text](image-74.png)

![alt text](image-75.png)

![alt text](image-76.png)

![alt text](image-77.png)

![alt text](image-78.png)

## Lab - `for` and `for generate`

### mux_generate
Simulation:
<br>![alt text](image-79.png)<br>

GLS:
<br>![alt text](image-81.png)<br>

Synthesis:
<br>![alt text](image-80.png)<br>

### demux_case
Simulation:
<br>![alt text](image-82.png)<br>
GLS:
<br>![alt text](image-84.png)<br>
Synthesis:
<br>![alt text](image-83.png)<br>

### demux_generate
Simulation:
<br>![alt text](image-85.png)<br>
GLS:
<br>![alt text](image-87.png)<br>
Synthesis:
<br>![alt text](image-86.png)<br>

### rca
Simulation:
<br>![alt text](image-88.png)<br>
GLS:
<br>![alt text](image-90.png)<br>
Synthesis:
<br>![alt text](image-89.png)<br>