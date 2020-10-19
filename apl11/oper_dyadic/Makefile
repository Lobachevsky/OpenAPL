# Makefile for oper_dyadic (dyadic operators)

include ../include/makefile.common

OBJECTS = ex_iprod.o ex_oprod.o ex_asgn.o

Q.o:	$(OBJECTS)
	$(LD) -r -o Q.o $(OBJECTS)

$(OBJECTS):	../include/apl.h

ex_asgn.o:	../include/char.h

.c.o:
	$(CC) $(CFLAGS) -c $<

