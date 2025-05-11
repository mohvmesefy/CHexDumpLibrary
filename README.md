# CHexDumpLibrary
C Hex Dump library. Prints hex dump from memory or file.<br/>
C89, C99 and >C99 compatible, CPP98 and >CPP98 compatible, Embedded C compatible.

Example of use

```c
#include "../CHexDump/CHexDump.h"


int main(int argc, char* argv[])
{
    unsigned char data[] = {
        0xDE, 0xAD, 0xBE, 0xEF, 0x48, 0x65, 0x6C, 0x6C,
        0x6F, 0x20, 0x57, 0x6F, 0x72, 0x6C, 0x64, 0x21,
        0x0A, 0x00, 0xFF
    };

    /* 1. Print hexdump from memory array */
    printf("HEXDUMP of memory array:\n");
    HEXDUMP_Memory(data, sizeof(data), 0);

    printf("\n");

    /* 2. Print hexdump from file if given */
    printf("HEXDUMP of file: %s\n", "c:\\A\\nslkv.txt");
    HEXDUMP_File("c:\\A\\nslkv.txt");

    return 0;
}
```


# History of changes ...
