#
# Makefile pentru lucrarea de laborator 4
#

CC = gcc
CFLAGS = -Wall -g -O
AR = ar

LIBLAB = liblab4.a

TEMPFILES = core core.* *.o temp.* *.out typescript* foo bar
PROGS =	access changemod filetype umask

OBJS = error.o

all: ${PROGS}

access: access.c $(LIBLAB)
	$(CC) -o $@ $?

changemod: changemod.c $(LIBLAB)
	$(CC) -o $@ $?

filetype: filetype.c $(LIBLAB)
	$(CC) -o $@ $?

umask: umask.c $(LIBLAB)
	$(CC) -o $@ $?

lib: ${OBJS}
	${AR} rcs ${LIBLAB} $<

clean:
	rm -f ${PROGS} ${TEMPFILES} ${LIBLAB}
