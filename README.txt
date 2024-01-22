# 8 bit CPU of following design -
	1. supports 32kB of primary memory
	2. 8 bit Program Counter
	3. 6 register - 
		a) 4 general purpose register (three 8 bit registers{R1, R2, R3}, one 16 bit register{E1})
		b) 1 stack pointer
		c) 1 flag register - Zero bit, Negative bit, Carry bit, Overflow bit

## Instruction Set
	Supports 3 addressing modes - 
		a) Immediate addressing mode
		b) Pointer addressing mode
		c) Implied addressing mode

1. MOV <Rn1> <Rn2>  ---> Rn1 = Rn2
2. MOV <E1> <Rn>    ---> E1 = Rn
3. ADD <Rn1> <Rn2>  ---> Rn1 = Rn1 + Rn2
4. ADD <E1> <Rn>    ---> E1 = E1 + Rn
5. SUB <Rn1> <Rn2>  ---> Rn1 = Rn1 - Rn2
6. SUB <E1> <Rn>    ---> E1 = E1 - Rn
7. MUL <Rn1> <Rn2>  ---> Rn1 = Rn1 * Rn2
8. MUL <E1> <Rn>    ---> E1 = E1 * Rn
9. LOAD <Rn> 0xHHLL ---> Rn <- [0xHHLL]
10. NOP             ---> No Operation