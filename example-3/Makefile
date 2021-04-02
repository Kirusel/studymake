# Усложненный make-file 3. 

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = Kazino-Royal
DEBUG_EXEC    = Kazino-Royal-dbg
SOURCE        = Kazino-Royal.cpp

all: debug release

debug: $(DEBUG_EXEC)

$(DEBUG_EXEC): $(SOURCE)
	g++ $(DEBUG_FLAGS) $(SOURCE) -o $@ -std=c++11

release: $(RELEASE_EXEC)

$(RELEASE_EXEC): $(SOURCE)
	g++ $(RELEASE_FLAGS) $(SOURCE) -o $@ -std=c++11

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)

