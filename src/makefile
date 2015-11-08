# a variavel objects contem todos os .o
# necessarios para compilar o projeto
objects = pmt.o sellers.o aho.o utils.o boyer_moore.o

# a variavel CC vai ser o compilador utilizado
CC=g++
# CFLAGS vao ser as opcoes passadas pro compilador
CFLAGS=-g -c -Wall

pmt: $(objects)
	$(CC) -o ../bin/pmt $(objects)

pmt.o: utils.h algs.h
sellers.o: algs.h
aho.o: algs.h
utils.o: utils.h
boyer_moore.o: algs.h

.PHONY: clean

clean:
	rm $(objects)