.PHONY: show-assembly show-assembly-with-source-code

all: simple.s simple.o show-assembly-with-source-code show-assembly

show-assembly-with-source-code: simple.o
	objdump -d -S simple.o

show-assembly: simple.s
	cat simple.s

simple.o: simple.c
	gcc -g -c simple.c

simple.s: simple.c
	gcc -S -O0 simple.c
