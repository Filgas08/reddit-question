include .env

CFLAGS = -std=c++11 -I. -I$(INCLUDE_PATH)include
LDFLAGS = -L$(INCLUDE_PATH)lib -lglfw3 -lGL -lGLU -lX11 -lXxf86vm -lXrandr -lpthread -lXi -lvulkan

a.out: *.cpp *.hpp
	g++ $(CFLAGS) -o a.out *.cpp $(LDFLAGS)

.PHONY: test clean

test: a.out
	./a.out

clean:
	rm -f a.out
