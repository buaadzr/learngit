.PHONY: clean PATH
main: main.o fun1.o fun2.o PATH
	gcc -o main main.o fun1.o fun2.o -L. -ldylib -L ./lib 
main.o: 
	gcc -c ./src/main.c -o main.o -I ./include
fun1.o: 
	gcc -c ./src/fun1.c -o fun1.o -I ./include
fun2.o:
	gcc -c ./src/fun2.c -o fun2.o -I ./include
PATH: 
	export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:./lib
clean:
	rm task main.o fun1.o fun2.o
