## Makefile
## Created     : 2024. 11. 06.
## Last updated: 2024. 11. 06.

rootFile = main.cc

inputFile = $(rootFile)

objectFile = $(inputFile:.cc=.o)
dependFile = $(inputFile:.cc=.d)

COMPILER = g++

default: all

all: $(objectFile)
	$(COMPILER) $(LINK_OPTION) $(INC_DIR) $(objectFile) $(ALL_LIBS) -o opentcad
	rm -f *~

%.o: %.cc
	$(COMPILER) $(COMPILE_OPTION) $(INC_DIR) -c $< -o $@

%.d: %.cc
	$(COMPILER) -M $(COMPILE_OPTION) $(INC_DIR) -c $< > $@
