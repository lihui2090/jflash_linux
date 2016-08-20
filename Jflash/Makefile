CC    = gcc
CFLAGS = -O2 -s

all: Jflash-s3c2440

Jflash-s3c2440: jtag.o k9sxx08.o pin2440.o ppt.o sjf.o
	$(CC) $(CFLAGS) -o $@ jtag.o k9sxx08.o pin2440.o ppt.o sjf.o

clean:
	rm -f *.o Jflash-s3c2440
