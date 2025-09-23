## Day 2 - Timing libs, hierarchical vs flat synthesis and efficient flop coding styles
### Intro to timing .lib files
_Tip: use_ `:syn off` _to disable syntax highlighting in vim editor_

Library Naming convention:

![alt text](image.png)

Timing info example for AND2 gate:

![alt text](image-1.png)

Drive strength variation in 2 input AND gate:

![alt text](image-2.png)

### Hierarchical vs Flat Synthesis
Synthesising multiple_modules.v in default mode:

![alt text](image-4.png)

using `flatten` (after synth) to convert hier to flattened netlist:

![alt text](image-3.png)

hier vs flattened netlist:

![alt text](image-5.png)

Synthesising sub module instead of top module:

![alt text](image-6.png)

#### Why synthesize sub-module individually?
- more efficient if multiple instances of same module are present. can synthesize one and instantiate multiple times.

- direct the tool to focus and handle smaller designs if it struggles with top module synthesis directly.

### Flop Coding Styles and optimization

#### Types of flops
- posedge clk with async reset
- posedge clk with async set
- posedge clk with sync reset
- posedge clk with sync set
- negedge clk with async reset
- negedge clk with async set
- negedge clk with sync reset
- negedge clk with sync set

_NOTE:_ sync reset can be thought of muxing the D input with the reset/set value

![alt text](image-7.png)

#### Flops Lab
Different flop types behaviour in waveform:

![alt text](image-8.png)
