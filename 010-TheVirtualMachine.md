# The Virtual Machine

## Registers

* PC - Virtual Machine Program Counter
* IP - FORTH Instruction Pointer
* WA - FORTH Word Address Pointer
* SP - FORTH Stack Pointer
* RP - FORTH Return Stack Pointer
* UP - FORTH User Area Pointer

## FORTH PRIMITIVES

## INTERFACE TO THE WORLD

```FORTH
: _SYSCALL ([param ...] SysCallID -- [result ...] Flag) ;
```
