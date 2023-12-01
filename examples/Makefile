SRC = $(wildcard *.c)
TAR = $(SRC:.c=.o)

.PHONE: all clean

all: $(TAR)

%.o: %.c
	clang-11 -O2 -target bpf -I ../includes -c $< -o $@

clean:
	rm -f $(TAR)
