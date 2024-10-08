# EX-4-ADVANCED-ENCRYPTION-STANDARD-DES-ALGORITHM

## Aim:
  To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

## ALGORITHM: 
  1. AES is based on a design principle known as a substitution–permutation. 
  2. AES does not use a Feistel network like DES, it uses variant of Rijndael. 
  3. It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits. 
  4. AES operates on a 4 × 4 column-major order array of bytes, termed the state

## PROGRAM: 

```
NAME : ROOP SAGAR S L
REG.NO : 212223040175
```
```
#include <stdio.h>
#include <string.h>
void xor_encrypt_decrypt(char *input, char *key) {
int input_len = strlen(input);
int key_len = strlen(key);
for (int i = 0; i < input_len; i++) {
input[i] = input[i] ^ key[i % key_len]; // XOR encryption
}
}
int main() {
printf("\n\n***** ADVANCED-ENCRYPTION STANDARD-DES-ALGORITHM *****");
printf("\n\n");
char url[] = "RoopSagarsl";
char key[] = "secretkey"; // Simple key for XOR encryption
printf("Original Text: %s\n", url);
xor_encrypt_decrypt(url, key);
printf("Encrypted Text: %s\n", url);
xor_encrypt_decrypt(url, key);
printf("Decrypted URL: %s\n", url);
return 0;
}
```
## OUTPUT:

![Screenshot 2024-10-07 111337](https://github.com/user-attachments/assets/0234063f-c840-41e6-bb1b-8e8698fb04d9)


## RESULT: 
