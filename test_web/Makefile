CC = g++
CFLAGS = -O2 -Wall -I .

# This flag includes the Pthreads library on a Linux box.
# Others systems will probably require something different.
LIB = -lpthread

all: main

main: main.o http_conn.o
	$(CC) $(CFLAGS) -o main main.o http_conn.o $(LIB)

main.o:
	$(CC) $(CFLAGS) -c main.cpp

http_conn.o:
	$(CC) $(CFLAGS) -c http_conn.cpp



clean:
	rm -f *.o main *~
	