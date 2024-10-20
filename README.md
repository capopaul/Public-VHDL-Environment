# vhdl-env

# Setup
- install hgdl
- install gtkwave

- to analyse a vhdl file : `ghdl -a your_file.vhdl`
- to compile your vhdl **entity** : `ghdl -e your_entity`
- to run your testbench : `ghdl -r testbench --stop-time=5us --vcd=testbench.vcd`
- to open it with GTKwave : `gtkwave testbench.vcd`

# Productive Environment
- install Visual Studio Code

In Visual Studio Code:
- install `VHDL` extension from Pu Zhao
- install `VHDL Formatter` extension from Vinrobot
