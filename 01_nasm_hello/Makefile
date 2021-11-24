srcs=$(wildcard *.asm)
objs=$(srcs:%.asm=%.o)

all:
	nasm -f elf $(srcs)
	ld -m elf_i386 -s -o hello $(objs)
clean:
	rm *.o hello
