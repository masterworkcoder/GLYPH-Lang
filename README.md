# m-lang
A micro programming language designed to be minimal and freestanding intended for osdev and general purpose use.

### Examples
Kernel
```
; include multiboot specification
import "asm/multiboot"

; Create a pointer to video memory
dec vid_mem:pointer void = 0xB8000

; Create the kernel main
dec kernel_main:func void(void)

; Write a character to video memory
*vid_mem = 'c'

end func
```

General Purpose
```
import "io"

dec main:func void(void)

print("Hello World\n")

end func
```
