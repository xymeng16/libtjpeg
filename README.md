# libtjpeg
libtjpeg is a trusted version of [libjpeg](http://libjpeg.sourceforge.net/) running on Intel SGX environment.  
Up to now, this library can be compiled as a static library with the Intel SGX C library, however, command I/O and FILE I/O are currently disabled given that it is impossible in the enclave. Thus, the **backing-store files** characteristic of libjpeg, which allows it to use disk space and files as buffer to load large image that your main memory and virtual memory cannot store continuously. I may write a OCALL wrapper later to implement the full-stack I/O function and replace the naive C standard I/O code in the libjpeg, but not now. (quitely busy in recent days:()
## Compilation
TBA  
The original README of libjpeg is [here](https://github.com/xymeng16/libtjpeg/blob/main/README).
