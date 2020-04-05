# Усложненный make-file.  Введены переменные для параметров компиляции и исполняемых файлов

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = hello
DEBUG_EXEC    = hello-dbg
INPUT_FILE	  = hello.cpp
#SOURCE        =

all: debug release

debug: $(DEBUG_EXEC)

hello-dbg: $(INPUT_FILE)
	g++ $(DEBUG_FLAGS) $(INPUT_FILE) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

hello: $(INPUT_FILE)
	g++ $(RELEASE_FLAGS) $(INPUT_FILE) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)

