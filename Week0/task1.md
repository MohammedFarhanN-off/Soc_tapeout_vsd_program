
# Chip Design & Soc Flow

## O0 – GCC Compiler

    A C testbench is compiled using the GCC compiler.

## O1 – Specification

    Defines the IC specifications: chip functions, architecture, and performance targets.
    The C testbench executable is applied to check specification correctness.

## O2 – RTL Development

    The chip design is described in Verilog RTL (Register Transfer Level) or other HDL

| Processor | Periperals |
| :-------- | :--------- |
| Gate level Netlist `syntesizable RTL`| Macros `synthesizable RTL` ,Analog Ip's `Functional RTL`|

    The C testbench executable validates RTL against the specification.

## O3 – SoC Integration & ASIC Flow

    Additional components are integrated with RTL: Macros , Analog IPs 
    ASIC design flow steps: 
    - Synthesis
    - Floorplanning
    - Placement
    - Routing
    - Clock tree synthesis
    - GDSII generation with DRC/LVS checks.
    The C testbench executable verifies the integrated SoC at this stage.

## O4 – Fabricated Chip & Applications

    The final chip operates in the 100–130 MHz frequency range.
    Deployed in products like:
    - iWatch (wearables)
    - Arduino boards (development/prototyping)
    - TV panels (consumer electronics)
    - AC appliances (home systems)
    - The C testbench executable confirms proper functioning in real-world applications.
    
## O0 = O1 = O2 = O3 = O4

    To ensure successful chip modeling and implementation, all stages — O0 (GCC Compiler) through O4 (Fabricated Applications) — must be executed correctly, with the C testbench applied equally at every stage for validation.




