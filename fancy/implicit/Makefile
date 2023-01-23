# This is done for c compilation. It is not recommended to use them this way because the might be a little bit confusing

# Compliling a C program : n.o is made automatically form n.c with 
# 	$(CC) -c #(CPPFLAGS) $(CFLAGS) $^ -o $@


# Compliling a C++ program : n.o is made automatically form n.cc with 
# 	$(cxx) -c #(CPPFLAGS) $(CXXLAGS) $^ -o $@

# Linking a single object file: n is made automatically from n.o by running the command $(CC) $(LDFLAGS) $^ $(LOADLIBES) $(LDLIBS) -o $@
# The important variables used by implicit rules are:

#CC: Program for compiling C programs; default cc
#CXX: Program for compiling C++ programs; default g++
#CFLAGS: Extra flags to give to the C compiler
#CXXFLAGS: Extra flags to give to the C++ compiler
#CPPFLAGS: Extra flags to give to the C preprocessor
CC = gcc # Flag for implicit rules
CFLAGS = -g # Flag for implicit rules. Turn on debug info

# Implicit rule #1: blah is built via the C linker implicit rule
# Implicit rule #2: blah.o is built via the C compilation implicit rule, because blah.c exists
blah: blah.o

blah.c:
	echo "int main() { return 0; }" > blah.c

clean:
	rm -f blah*
