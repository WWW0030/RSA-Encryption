# RSA Encryption and Decryption Documentation

This documentation provides an overview of the three Java programs: `encrypt2`, `Decryption`, and `Challenge2`, which implement RSA encryption and decryption. RSA is a widely-used public-key cryptosystem that allows secure data transmission and encryption.

## `encrypt2` - RSA Encryption

### Program Description
`encrypt2` is a Java program that performs RSA encryption on user-provided files. It generates random prime numbers `p` and `q`, calculates the modulus `n`, totient `t`, public exponent `e`, and private exponent `d`. The program reads characters from an input file, encrypts them using RSA, and writes the resulting integers to an output file.

### Usage
1. Compile and run the program.
2. Enter prime numbers `p` and `q` as prompted.
3. The program will generate public key `(n, e)` and private key `d`.
4. The input file (specified in the code) is read character by character and encrypted.
5. The encrypted integers are written to the output file.

## `Decryption` - RSA Decryption

### Program Description
`Decryption` is a Java program that performs RSA decryption given the private key `(n, d)` and the ciphertext from an input file. It reads the encrypted integers from an input file, decrypts them using RSA, and writes the resulting characters to an output file.

### Usage
1. Compile and run the program.
2. Enter the values of `n`, `e`, and `d` as prompted.
3. The program reads encrypted integers from the input file (specified in the code).
4. It decrypts the integers using RSA with the provided private key.
5. The decrypted characters are written to the output file.

## `Challenge2` - RSA Challenge Decryption

### Program Description
`Challenge2` is a Java program designed to decrypt an RSA-encrypted message when only given `n` and `e`. It first attempts to find the prime factors `p` and `q` of `n` by searching for pairs of prime numbers whose product equals `n`. Once `p` and `q` are found, it calculates `t` and computes the private exponent `d` using a brute-force method. Finally, it decrypts the message and outputs the original text.

### Usage
1. Compile and run the program.
2. Enter the values of `n` and `e` as prompted.
3. The program attempts to find the prime factors `p` and `q` of `n`.
4. It calculates `t` and then tries to find `d`.
5. The program reads encrypted integers from the input file (specified in the code).
6. It decrypts the integers using RSA with the calculated private key.
7. The decrypted characters are written to the output file.

## Important Notes
- The input and output file paths are specified in the code and should be adjusted as needed.
- These programs are simplified for educational purposes and may not handle all edge cases or security considerations of a real-world RSA implementation.
- RSA encryption and decryption are typically performed with much larger key sizes for security.
