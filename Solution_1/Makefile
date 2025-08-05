# Compiler
CXX = g++
CXXFLAGS = -std=c++11 -Wall -Wextra

# Target executable
TARGET = ColorCoder

# Source files
SRCS = main.cpp ColorPair.cpp ColorMap.cpp

# Header dependencies (optional, not strictly needed unless for dependency checking)
HEADERS = ColorPair.h ColorMap.h

# Object files (same names as source files, but with .o extension)
OBJS = $(SRCS:.cpp=.o)

# Default target
all: $(TARGET)

# Linking
$(TARGET): $(OBJS)
	$(CXX) $(CXXFLAGS) -o $@ $^

# Compilation rule
%.o: %.cpp $(HEADERS)
	$(CXX) $(CXXFLAGS) -c $< -o $@

# Clean rule
clean:
	rm -f $(OBJS) $(TARGET)

