# 0x0E. C - Structures, typedef

## Resource

- [0x0d. Structures](../references/Structures.pdf)
- [struct (C programming Language)](https://en.wikipedia.org/wiki/Struct_(C_programming_language))
- [struct memory layout in C](https://stackoverflow.com/questions/2748995/struct-memory-layout-in-c)
- [Betty Documentation Style: Data Structures](https://github.com/holbertonschool/Betty/wiki/Documentation:-Data-structures)
- [0x0d typedef](../references/typedef.pdf)
- [Programming in C by Stephen Kochan Chapter 8, working with Structures pg 163-189](../references/Programming_in_C_4th_Edition_by_Stephen_Kochan.pdf) \- stephen g. kochan\(1\).pdf)
- [The Lost Art of C Structure Packing](http://www.catb.org/esr/structure-packing/) ***Advanced, not mandatory***

## Tasks

0. [Poppy](./dog.h) : A new type `struct dog` with the following elements. <img align="right" src="../.imgs/dog0.jpg" alt="dog0" width="120" height="120">
	- `name`, type = `char *`
	- `age`, type = `float`
	- `owner`, type = `char *`
	- Compile the code this way: `gcc -Wall -pedantic -Werror -Wextra -std=gnu89 0-main.c -o a`
1. [A dog is the only thing on earth that loves you more than you love yourself](./1-init_dog.c) : A function that initialize a variable of type `struct dog`<img align="right" src="../.imgs/dog1.jpg" alt="dog1" width="120" height="120">
	- Prototype: `void init_dog(struct dog *d, char *name, float age, char *owner);`
	- Compile the code this way: `gcc -Wall -pedantic -Werror -Wextra -std=gnu89 1-main.c 1-init_dog.c -o b`
2. [A dog will teach you unconditional love. If you can have that in your life, things won't be too bad](./2-print_dog.c) : A function that prints a `struct dog`<img align="right" src="../.imgs/dog2.jpg" alt="dog1" width="120" height="120">
	- Prototype: `void print_dog(struct dog *d);`
	- Format: see example below.
	- You are allowed to use the standard library.
	- If an element of `d` is `NULL`, print `(nil)` instead of this element. (if `name` is `NULL`, print `Name: (nil)`)
	- If `d` is `NULL` print nothing.
	- Compile the code this way: `gcc -Wall -pedantic -Werror -Wextra -std=gnu89 2-main.c 2-print_dog.c -o c`