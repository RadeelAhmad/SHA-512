# SHA-512 Implementation in C
This repository contains a C implementation of the SHA-512 cryptographic hash function. SHA-512 is part of the SHA-2 family, which is used in various security applications and protocols, including TLS and SSL, PGP, SSH, and more.

## Overview
The provided C code implements the SHA-512 algorithm and includes functions for compressing message blocks and calculating the final hash value. The code also allows users to specify a round number to display intermediate hash values for a specific round.

## Features
- **Circular Right Shift:** Implements the circular right shift operation used in SHA-512.
- **SHA-512 Functions:** Defines core SHA-512 functions including Ch, Maj, Sigma0, Sigma1, sigma0, and sigma1.
- **Compression Function:** Implements the SHA-512 compression function to process message blocks.
- **Padding and Message Processing:** Handles padding and processes message blocks according to SHA-512 specifications.
- **User Interaction:** Accepts user input for the message and round number, displaying intermediate and final hash values.

## Usage
**Compilation**
To compile the code, use a C compiler such as `gcc`:

```bash
gcc -o sha512 sha512.c
```

**Running the Program**
Run the compiled program with:

```bash
./sha512
```

You will be prompted to enter the text message and the round number. The program will then output the intermediate hash values for the specified round and the final hash value.

**Example**
```console
Enter the text: Hello, world!
Enter the round number: 10
values for round 10:
H[0] = 6a09e667f3bcc908
H[1] = bb67ae8584caa73b
H[2] = 3c6ef372fe94f82b
H[3] = a54ff53a5f1d36f1
H[4] = 510e527fade682d1
H[5] = 9b05688c2b3e6c1f
H[6] = 1f83d9abfb41bd6b
H[7] = 5be0cd19137e2179
Final hash value:
6a09e667f3bcc908bb67ae8584caa73b3c6ef372fe94f82ba54ff53a5f1d36f1510e527fade682d19b05688c2b3e6c1f1f83d9abfb41bd6b5be0cd19137e2179
```
