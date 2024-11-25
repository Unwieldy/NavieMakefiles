# Compiler to be used
CXX = g++

# Compiler flags
CFLAGS = -Wall -Wextra -std=c++23

# Target executable file name
TARGET = hello

# Source files
SRCS = hello.cpp fisk.cpp

# Object files
OBJS = $(SRCS:.cpp=.o)

# Default goal
all: $(TARGET)

# Link the object files to create the executable
$(TARGET): $(OBJS)
	$(CXX) $(CFLAGS) -o $(TARGET) $(OBJS)

# Compile the source files into object files
%.o: %.cpp
	$(CXX) $(CFLAGS) -c $< -o $@

# hello.o: hello.cpp
# 	$(CXX) $(CFLAGS) -c hello.cpp -o hello.o
#
# fisk.o: fisk.cpp
# 	$(CXX) $(CFLAGS) -c $< -o $@



# Clean up generated files
clean:
	rm -f $(OBJS) $(TARGET)

.PHONY: all clean
