# Welcome to My Readline
This was arduous

## Task
Task istself is a big challange. Task was recreating readline function using only limited functions.

## Description
I stucked it for more than 1 month, probably 2 months. Today i created a simple function that stips from end of the string. And this is it! my code worked finally.

## Installation
Nothing to install. Just use it as ordinary functions.

## Usage
You give it int value that identificator of an open file. Every time you call it with the same identificator it returns by 1 full line till it reaches the EOF.
```
  int READLINE_READ_SIZE = 512;
  
  int main(int ac, char **av)
  {
    char *str = NULL;
  
    int fd = open("./file.txt", O_RDONLY);
    while ((str = my_readline(fd)) != NULL)
    {
        printf("%s\n", str);
        free(str);
    }
    close(fd);
    //
    //  Yes it's also working with stdin :-)
    //  printf("%s", my_readline(0));
    //
  
    return 0;
  }
```

### The Core Team


<span><i>Made at <a href='https://qwasar.io'>Qwasar SV -- Software Engineering School</a></i></span>
<span><img alt='Qwasar SV -- Software Engineering School's Logo' src='https://storage.googleapis.com/qwasar-public/qwasar-logo_50x50.png' width='20px'></span>
