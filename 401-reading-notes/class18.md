# Encryption, Decryption & Hacking

The need for encryption
- Encrypting data means that we scramble the original data to hide the meaning of the text, while still making it possible for the data to be unscrambled using a secret key.
Encryption enables two people (or computers!) to share private information over open networks.

Encryption, decryption, and cracking
- The Caesar Cipher is a simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount.

Symmetric encryption techniques
- A symmetric encryption is any technique where the same key is used to both encrypt and decrypt the data. The Caesar Cipher is one of the simplest symmetric encryption techniques, and of course, one of the easiest to crack.

# Caesar cipher


The Caesar cipher is a classic example of ancient cryptography and is said to have been used by Julius Caesar. The Caesar cipher is based on transposition and involves shifting each letter of the plaintext message by a certain number of letters, historically three, as shown in Figure 5.1. The ciphertext can be decrypted by applying the same number of shifts in the opposite direction. This type of encryption is known as a substitution cipher, due to the substitution of one letter for another in a consistent fashion.

![](https://ars.els-cdn.com/content/image/3-s2.0-B9780128007440000051-f05-01-9780128007440.jpg)

Breaking the cipher
- The Caesar cipher can be easily broken even in a ciphertext-only scenario. Two situations can be considered:

1. an attacker knows (or guesses) that some sort of simple substitution cipher has been used, but not specifically that it is a Caesar scheme;
2. an attacker knows that a Caesar cipher is in use, but does not know the shift value.

Notes taken from
1. https://en.wikipedia.org/wiki/Caesar_cipher
2. https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/the-need-for-encryption
3. https://www.sciencedirect.com/topics/computer-science/caesar-cipher#:~:text=The%20Caesar%20cipher%20is%20based,shifts%20in%20the%20opposite%20direction.