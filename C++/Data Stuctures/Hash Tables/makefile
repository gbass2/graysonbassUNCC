CC = g++
CFLAGS = -I. --std=c++11
OBJS = anagram_test.o anagram.o
TARGET = hash

.PHONY : clean run all

all: clean $(TARGET) run

%.o: %.cpp
	$(CC) -c -o $@ $< $(CFLAGS)

$(TARGET) : $(OBJS)
	$(CC) -o $@ $^ $(CFLAGS)

clean:
	rm -rf $(TARGET)
	rm -rf *.o

run:
	./$(TARGET)
