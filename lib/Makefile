AR = ar
CC = clang
CFLAGS = -g -Wall -I../include
OUTPUT = libfuncs.a
OBJFILES = func1.o func2.o
.PHONY: clean

$(OUTPUT): $(OBJFILES)
	$(AR) rv $(OUTPUT) $(OBJFILES)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJFILES) $(OUTPUT)
