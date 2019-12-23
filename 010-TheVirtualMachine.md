# THE VIRTUAL MACHINE

## REGISTERS

* PC - Virtual Machine Program Counter
* IP - FORTH Instruction Pointer
* WA - FORTH Word Address Pointer
* SP - FORTH Stack Pointer
* RP - FORTH Return Stack Pointer
* UP - FORTH User Area Pointer

## FORTH PRIMITIVES

## INTERFACE TO THE WORLD

```
0 CONSTANT _KEY_
1 CONSTANT _EMIT_
2 CONSTANT _QTERM_
3 CONSTANT _FOPEN_
4 CONSTANT _FCLOSE_
5 CONSTANT _FREAD_
6 CONSTANT _FWRITE_
7 CONSTANT _BLKRW_



: SYSCALL ( [param ...] SysCallID -- [result ...] Flag ) ;

: (KEY) ( -- key )   _KEY_ SYSCALL DROP ;

: (EMIT) ( ch -- )   _EMIT_ SYSCALL DROP ;   
```
