VERSION = "4.0.0"

#---------------------------------------------------------------------------------
# options for code generation
#---------------------------------------------------------------------------------
CC=g++
CFLAGS=-g -O2 -Wall -D__BUILD_DATE="\"`date +'%Y%m%d'`\"" -D__BUILD_VERSION="\"$(VERSION)\""

SOURCES=constify.cpp
OBJS=constify.o
EXE=constify.exe
DEFINES = 
LIBS = 
#---------------------------------------------------------------------------------
all: $(EXE)

#---------------------------------------------------------------------------------
$(EXE) : $(OBJS)
	@echo make exe $(notdir $<) 
	$(CC) $(CFLAGS)  $(OBJS) -o $@
	
constify.o : constify.cpp
	@echo make obj $(notdir $<) 
	$(CC) $(CFLAGS) -c $<

lzss.o : lzss.c
	@echo make obj $(notdir $<) 
	$(CC) $(CFLAGS) -c $<

#---------------------------------------------------------------------------------
clean:
	rm -f *.o *.exe 


