CC := g++ -std=c++11 

CFLAGS := -g -Wall -gstabs+

TARGET := test

SRCS := $(wildcard *.cpp)
OBJS := $(patsubst %cpp,%o,$(SRCS))

all:$(TARGET)

%.o:%.cpp
	$(CC) $(CFLAGS) -c $<

$(TARGET):$(OBJS)
	$(CC) $(CFLAGS) -o $@ $^

clean:
	rm -rf $(TARGET) *.o *.txt
	
