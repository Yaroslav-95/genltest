all: genltest.c
	gcc genltest.c $(shell pkg-config --cflags --libs libnl-3.0 libnl-genl-3.0) -o genltest
