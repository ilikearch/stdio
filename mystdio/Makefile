# 定义变量
CC = gcc
CFLAGS = -Wall -g
OBJ = main.o my_stdio.o
TARGET = my_stdio

# 默认目标
all: $(TARGET)

# 链接目标
$(TARGET): $(OBJ)
	$(CC) -o $@ $^

# 编译源文件
%.o: %.c my_stdio.h
	$(CC) $(CFLAGS) -c $<

# 清理生成的文件
clean:
	rm -f $(OBJ) $(TARGET)

# 伪目标
.PHONY: all clean

