CFLAGS = -O2

CC	=	gcc

OBJS = mkvcdfs.o vcdisofs.o edc_ecc.o

# Default Dependencies
%.obj: %.c
	$(CC) $(CCFLAGS) -c -o $@ $<


all:	mkvcdfs.exe vcdmplex.exe

mkvcdfs.exe: $(OBJS)
	gcc -o mkvcdfs.exe -Zbin-files $(OBJS)

vcdmplex.exe: vcdmplex.c
	gcc -O2 -o vcdmplex.exe -Zbin-files vcdmplex.c

clean:
	rm -f *.o mkvcdfs.exe vcdmplex.exe
