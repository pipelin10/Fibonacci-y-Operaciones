clean:
	rm -rf a.out oper.o liboper.a main
obj:
	gcc -c oper.c -o oper.o
lib:
	ar rcs liboper.a oper.o
bin: obj lib
	gcc -static main.c -L. -I. -loper -o main
