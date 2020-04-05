# Усложненный make-file.  Введены переменные для параметров компиляции и исполняемых файлов

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = Kazino-Royal
DEBUG_EXEC    = Kazino-Royal-dbg
INPUT_FILE	  = Kazino-Royal.cpp
#SOURCE        =

all: debug release clean

debug: $(DEBUG_EXEC)

Kazino-Royal-dbg: $(INPUT_FILE)
	g++ $(DEBUG_FLAGS) $(INPUT_FILE) -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

Kazino-Royal: $(INPUT_FILE)
	g++ $(RELEASE_FLAGS) $(INPUT_FILE) -o $(RELEASE_EXEC)

clean:
	rm -f $(DEBUG_EXEC)

