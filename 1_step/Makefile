.SUFFIXES : .c .o

OBJS = main.o \
		  foo.o \
		  bar.o
SRCS = $(OBJS:.o=.c)

CC = gcc
CFLAGS = -g -c
INC = -I~/workspace/make_tutorial/1_step/Header

TARGET = test

$(TARGET): $(OBJS)
	$(CC) -o $(TARGET) $(OBJS)


clean:
	rm -rf $(OBJS) $(TARGET) core

main.o: foo.h bar.h main.c
foo.o: foo.h foo.c
bar.o: bar.h bar.c

