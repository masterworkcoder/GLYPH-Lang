# GLYPH
A programming language designed to be minimal and freestanding intended for osdev and general purpose use.

Currently there is only a small standard library planned to do some very basic things.
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
; The io library is simply a possible standard library
import "io"

dec main:func void(void)

print("Hello World\n")

end func
```
