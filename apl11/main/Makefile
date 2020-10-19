# Makefile for main 

include ../include/makefile.common

OBJECTS = mainloop.o exit.o apl.o getinput.o

Q.o:	$(OBJECTS)
	$(LD) -r -o Q.o $(OBJECTS)

$(OBJECTS):	../include/apl.h

apl.o:	../include/patchlevel.h

getinput.o:	../include/config.h 

.c.o:
	$(CC) $(CFLAGS) -c $<

clean:
	rm -f $(OBJECTS) core

