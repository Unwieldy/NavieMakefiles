#Variables
CXX = g++
CXXFLAGS = -Wall -Wextra -pedantic -std=c++11
TARGET = hello
SRCS = hello.cpp fisk.cpp

# Rules
all: $(TARGET)

$(TARGET): $(SRCS)
	$(CXX) $(CXXFLAGS) $(SRCS) -o $(TARGET)

clean:
	rm -f $(TARGET)

.PHONY: all clean

