CFLAGS=-c -Wall -O2
CC=arm-linux-gnueabihf-gcc
AR=arm-linux-gnueabihf-ar

objs = main.o

all: main

main: $(objs)
	$(CC) $(objs) -o main

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@


clean:
	rm  -rf *.o  main

