# GET NEXT LINE
The aim of this project is to create a function able to read from a file descriptor. Additionally, this project is a good way to learn how to work properly with memory and what static variables are.

The function will return a pointer to the line just read or NULL if an error happens (e.g., the file descriptor is invalid or a problem occurred when trying to allocate memory). In this project, a line is considered to go from the last character read (or the beginning of the file descriptor) to the next newline character '\n', included (or the end of the file descriptor); this way, if you call the function enough times, you can extract all the information from the file descriptor. The amount of characters read using the function [read]([https://www.gnu.org/software/libc/manual/html_node/Function-Index.html](https://linux.die.net/man/2/read)) is defined as BUFFER_SIZE 5 and can be changed when compiling adding: `-D BUFFER_SIZE=`_newsize_

### Bonus
Compiling with bonus will allow the user to call the function with different file descriptors simultaneously.
