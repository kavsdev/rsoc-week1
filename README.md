# RISC-V Reference SoC Tapeout Program VSD - Week1
## [Day1](#day1---introduction-to-verilog-rtl-design-and-synthesis)
## [Day2](day2.md)
## [Day3](day3.md)
## [Day4](day4.md)
## [Day5](day5.md)

## Day1 - Introduction to Verilog RTL design and Synthesis
### skywater130 digital pdk setup
- make a `VLSI` directory in the home folder
- `cd VLSI`
- `git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git`
### simulating using iverilog and gtkwave
Running the simulator with design and tesbench files:
<img width="952" height="118" alt="image" src="https://github.com/user-attachments/assets/2a17b7d9-405c-4bdb-a5da-feb300d6aa09" />
Viewing design signals in gtkwave:
<img width="1920" height="1049" alt="image" src="https://github.com/user-attachments/assets/4e29facc-dd06-480e-9295-d17c4ba96241" />

### Yosys synthesis
Syntehsis tool: Takes in design .v file and pdk .lib file and produces a netlist file

`.lib file`: text file that describes the timing, power, and area characteristics of a standard cell library

Verifying the synthesis result:
<img width="1301" height="497" alt="image" src="https://github.com/user-attachments/assets/593dbf51-1bb1-48c1-8d79-beed35139925" />

Why we need different flavours of gate:
<img width="977" height="463" alt="image" src="https://github.com/user-attachments/assets/e9e05adc-940a-4055-8485-6c04e615930d" />

Why we need slow cells then?:
<img width="974" height="480" alt="image" src="https://github.com/user-attachments/assets/12e1b39c-2219-4363-9803-933552ff0d2c" />

Rule of thumb in choosing a speed variant:
<img width="832" height="229" alt="image" src="https://github.com/user-attachments/assets/b5a43bd4-43eb-4cfe-b6f4-2633ed86ff60" />

How Synthesis of RTL maps to gates and FF:
<img width="981" height="534" alt="image" src="https://github.com/user-attachments/assets/2fc4856f-0eff-4e42-8841-f133227c0e0b" />

### Yosys Lab
Invoking yosys from rtl work dir:

<img width="746" height="186" alt="image" src="https://github.com/user-attachments/assets/73ae943c-a710-4640-932a-15e60e2df606" />

Reading in lib file:

<img width="738" height="97" alt="image" src="https://github.com/user-attachments/assets/13df19aa-fb53-45aa-bd49-7a636042e1df" />

Reading in RTL:

<img width="703" height="134" alt="image" src="https://github.com/user-attachments/assets/13c110b3-c8b1-4903-ba44-9f955b2d2f76" />

Synthesising top module:

<img width="792" height="768" alt="image" src="https://github.com/user-attachments/assets/df7b6fed-dd68-4ed8-ac6a-cfb52faa96ef" />

Reading in lib cells with abc command:

<img width="1154" height="776" alt="image" src="https://github.com/user-attachments/assets/89e2829b-4117-4953-875c-db5eb0f1056c" />

Synthesis results:

<img width="684" height="163" alt="image" src="https://github.com/user-attachments/assets/ec447150-5a91-442e-925d-e38d41b8778d" />

using `show` to view schematic visualisation:

<img width="611" height="690" alt="image" src="https://github.com/user-attachments/assets/d7537c51-0f12-4eca-ae29-21b5635123a8" />

Write synthesised netlist with and without attribute comments:

<img width="611" height="425" alt="image" src="https://github.com/user-attachments/assets/e14e09e5-8cd1-41ad-ae0a-16f4a2a2fa10" />

Syntehsised netlist:

<img width="900" height="525" alt="image" src="https://github.com/user-attachments/assets/40cb6f5f-90ac-40d2-839d-d53671eb67b6" />




