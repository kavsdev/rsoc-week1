# Day 4 - GLS, blocking vs non-blocking and Synthesis-Simulation mismatch
## GLS, Synthesis-Simulation mismatch and Blocking/Non-blocking statements
<img src="image-38.png" width="400"/>
<br>
<img src="image-39.png" width="400"/>
<br>
NOTE: if the gate level models are delay annotated, the GLS can be used for timing validation.
<br>
<img src="image-40.png" width="400"/>
<br>

### synthesis simulation mismatch
<img src="image-41.png" width="400"/>
<br>
Left RTL infers a double edge flop during simulation <br>
Right RTL infers a mux during simulation <br>
Synthesis doesnt consider sensitivity list; infers mux both times

### Blocking And NonBlocking Statements In Verilog
<img src="image-42.png" width="400"/>
<br>
<img src="image-43.png" width="400"/>
<br>
always use non blocking statements when assigning sequential elements
![alt text](image-44.png)
<img src="image-44.png" width="400"/>
<br>

Left RTL infers a 1 cycle delay for the reg value <br>
Right RTL infers same cycle output <br>
synthesis doesnt care about the order of blocking statements, infers same cycle output <br>

## Lab - sensitiivity list

### ternary_operator_mux
Simulation:
<br><img src="image-46.png" width="400"/><br>
Synthesis:
<br><img src="image-45.png" width="400"/><br>
GLS:
<br><img src="image-47.png" width="400"/><br>

### bad_mux
RTL simulation and GLS:
<br><img src="image-48.png" width="600"/><br>
Synthesis:
<br><img src="image-49.png" width="400"/><br>

## Lab - blocking and non blocking
RTL simulation and GLS:
<br><img src="image-50.png" width="600"/><br>
Synthesis:
<br><img src="image-51.png" width="400"/><br>