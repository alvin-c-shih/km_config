# Makefile
.PHONY: all

#CC := gcc
CC := g++

#CFLAGS := -O3 -std=c++11 # use this option in case openmp does not work 
CFLAGS := -O3 -std=c++11 -fopenmp

all: km_config

km_config:../lib/km_config.cpp ../lib/km_config.h km_config_cl.cpp
	$(CC) $(CFLAGS) -o km_config km_config_cl.cpp 

.PHONY: clean
clean:
	$(RM) km_config
