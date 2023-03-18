CFLAGS = -Wall -g
PYTHON = python3.6

.DEFAULT_GOAL: all

.PHONY: all clean

all: main

main: main.o
	gcc main.o -o main -l$(PYTHON)m

main.o: main.c
	gcc -I/usr/include/$(PYTHON)/ -c main.c -o main.o

run:
	./main

clean:
	-rm -f main main.o
	-rm -f *~
