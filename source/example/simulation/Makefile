run:
	make clean;\
	if [ ! -d "./cache/" ]; then \
  		mkdir ./cache; \
	fi;\
	ghdl -a --workdir=./cache --std=08 ../rtl/none.vhd;\

	ghdl -a --workdir=./cache --std=08 testbench.vhd;\
	ghdl -e --workdir=./cache --std=08 testbench;\
	ghdl -r --workdir=./cache --std=08 testbench --stop-time=25us --vcd=./cache/testbench.vcd;
	
rungui:
	make run;\
	gtkwave ./cache/testbench.vcd;

clean:
	if [ -d "./cache/" ]; then \
  		rm -r ./cache; \
	fi;