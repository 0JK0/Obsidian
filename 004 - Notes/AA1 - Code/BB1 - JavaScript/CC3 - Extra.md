#JavaScript #Code  


# Following the Stuff Skipped at [[CC1 - Basics#!]]

## ^ Short Circuit

-> I have a deep hatred toward truth tables

-> Used when is necessary to use a logic but other past logic needs to also be **True**

	Const result = { user && user.name} || "Anonymus";
	// If user exist and has a name use it
	// Otherwayse default annonymus

## ^ Operators Bit-wise

-> Might Never need to use this is just calculations with binary


	// bit : 0 1
	// Byte: 8 bits
	// Byte: 00000000 -> 0
	// Byte: 00000001 -> 1
	// Byte: 00000010 -> 2
	// Byte: 00000011 -> 3
	// Byte: 00000100 -> 4
	// Byte: 00000101 -> 5
	// Byte: 00000110 -> 6

## ^ Ternarios

-> Just a more low level way of doing "If - Else", more try-hard

	// ? "si es True", : "Si es False", Le da valor a AX
	let AX = edad > 17 ? "Permitir" : "No ingresar";