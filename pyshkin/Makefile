create: pushkin.o main.o
	@gcc -c main.c -o main.o
	@gcc -fPIC -c pushkin.c -o pushkin.o
	@gcc main.o -o main.out -ldl
	@gcc -shared -o pushkin.so pushkin.o
compile: create
	@./main.out
clean:
	@rm -rf  *.o *.so