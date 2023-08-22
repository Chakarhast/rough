<div align="center">
  <h1 style="font-family: 'Helvetica', sans-serif;">Documentation</h1>
</div>

## Directory Structure

``` mathematica
Root Directory: with-bonus
├── launcher
│   ├── launch.c
│   └── makefile
├── loader
│   ├── loader.h
│   ├── loader.c
│   └── makefile
├── bin
├── test
│   ├── fib.c
│   └── makefile
└── makefile

```
## Folder: Loader
### loader.h

'loader.h' is a header file. It helps in including various libriaries.
``` C
#include <stdio.h>                 // Include standard input/output library.
#include <elf.h>                   // Include ELF file format definitions.
#include <string.h>                // Include string manipulation functions.
#include <fcntl.h>                 // Include file control options.
#include <stdlib.h>                // Include standard library functions.
#include <unistd.h>                // Include POSIX API for system calls.
#include <assert.h>                // Include assertion library.
#include <sys/types.h>             // Include data types for system calls.
#include <sys/mman.h>              // Include memory mapping functions.

void load_and_run_elf(char** exe);
void loader_cleanup();
```

Functions like load_and_run_elf and loader_cleanup are declared in a header file so that their declarations are visible to other source code files that include the header. 

