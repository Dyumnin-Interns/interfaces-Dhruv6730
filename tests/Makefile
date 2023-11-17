SIM ?= icarus
TOPLEVEL_LANG ?= verilog
VERILOG_SOURCES += $(PWD)/../hdl/dut.v
VERILOG_SOURCES += $(PWD)/../wrappers/ifc_test.v
VERILOG_SOURCES += $(PWD)/../hdl/FIFO2.v

dut:
	rm -rf sim_build
	$(MAKE) sim MODULE=ifc_test TOPLEVEL=ifc_test
include $(shell cocotb-config --makefiles)/Makefile.sim
