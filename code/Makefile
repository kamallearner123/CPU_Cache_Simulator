
CFLAGS=-Wall -Werror -c -g -fsanitize=address -lasan
main.o: main.c main.h
	gcc $(CFLAGS) main.c -o main.o

cache_sim: main.o 
	gcc -Wall -Werror main.o -o cache_sim -lasan

.DEFAULT_GOAL := cache_sim

clean: 
	rm -f main main.o
#all: cacheSim
#	echo "Compilation SUCCEEDED"
