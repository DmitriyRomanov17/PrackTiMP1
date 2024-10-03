.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC = casino
DEBUG_EXEC    = casino-dbg
SOURCE       = Kazino-Royal.cpp

# Default target
all: debug release

# Debug target
debug: $(DEBUG_EXEC)

# Release target
release: $(RELEASE_EXEC)

# Rules for building executables
$(DEBUG_EXEC): $(SOURCE)
	g++ $(DEBUG_FLAGS) $(SOURCE) -o $(DEBUG_EXEC)

$(RELEASE_EXEC): $(SOURCE)
	g++ $(RELEASE_FLAGS) $(SOURCE) -o $(RELEASE_EXEC)

# Clean target
clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)
