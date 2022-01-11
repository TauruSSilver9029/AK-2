CC=g++
CFLAGS=-c -W

run-calc: main.o calculator.o
	${CC} main.o calculator.o -o run-calc

main.o: main.cpp
	${CC} ${CFLAGS} main.cpp

calculator.a: calculator.cpp
	ar -rcs calculator.a calculator.o

calculator.o: calculator.cpp calculator.h
	${CC} ${CFLAGS} calculator.cpp

clean:
	rm *.o run-calc
