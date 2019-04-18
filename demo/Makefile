CFLAGS = -c -Wall -O2
CC = gcc
AR = ar
LD = ld

TOP=$(shell pwd)

INC_DIR = -I $(TOP)/include
LIK_DIR = -L $(TOP)/libs
LDFLAGS = -Wl,-rpath $(TOP)/libs
LIBS = -lpthread -ldl -lrt -luspsdk -lssl -lcrypto

object = main.c
OBJLIB = lib.so
TARGET = main

all: $(OBJLIB) $(TARGET)

$(TARGET): $(object)
	$(CC) $(object) $(INC_DIR) $(LIK_DIR) $(LIBS) $(LDFLAGS) -o $(TARGET)
	
$(OBJLIB): main.o
	$(CC) -shared -o -fPIC -o $@ $^

main.o: $(object)
	$(CC) $(object) $(INC_DIR) $(LIK_DIR) $(LIBS) -c -fPIC -o $@ 

.PHONY: clean

clean:
	-rm  -rf *.o $(OBJLIB) $(TARGET)

