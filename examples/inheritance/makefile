OBJECTS=main.o base.o derived.o
CC=g++
CFLAGS=-fno-diagnostics-color
LFLAGS=

prog:		$(OBJECTS)
		$(CC) -o prog $(OBJECTS) $(LFLAGS)

main.o:		main.cpp base.h derived.h
		$(CC) $(CFLAGS) -c main.cpp

base.o:		base.cpp base.h 
		$(CC) $(CFLAGS) -c base.cpp

derived.o:		derived.cpp derived.h base.h
		$(CC) $(CFLAGS) -c derived.cpp

clean:
		rm -rf $(OBJECTS)  prog *~
