

PROJNAME = example

CC = g++
CFLAGS = -Wall -c
LFLAGS = -Wall

LINK_LIBS = -framework glut -framework opengl


OBJS =  initShader.o append_example4.o
all: example


example: $(OBJS) 
	$(CC) $(LFLAGS) $(OBJS) -o $@ $(LINK_LIBS)

append_example4.o: append_example4.cpp Angel.h
	$(CC) $(CFLAGS) $<

initShader.o: initShader.cpp Angel.h
	$(CC) $(CFLAGS) $<


clean:
	\rm -f $(OBJS) $(PROJNAME)