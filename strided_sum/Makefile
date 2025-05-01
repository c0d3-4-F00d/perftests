# Makefile for Linux using GCC
# 
# For compiling with micorosft MSVC, use make.bat

CC = gcc
OPTFLAG = -Ofast
CFLAGS = -Wall $(OPTFLAG) -std=gnu11
OBJS = strided_sum.o
OUT = strided_sum

all: $(OUT)

$(OUT): $(OBJS)
	$(CC) -o $(OUT) $(OBJS)

strided_sum.o: strided_sum.c Makefile
	$(CC) $(CFLAGS) -DOPTFLAG=\"$(OPTFLAG)\" -c strided_sum.c

clean:
	rm -f *.o $(OUT)
