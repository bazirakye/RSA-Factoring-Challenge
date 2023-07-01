## RSA-Factoring-Challenge

RSA (Rivest-Shamir-Adleman) is a widely used public-key encryption algorithm that was invented by Ron Rivest, Adi Shamir, and Leonard Adleman in 1977. It is named after the initials of its inventors.

RSA encryption is based on the mathematical difficulty of factoring large composite numbers into their prime factors. The algorithm utilizes a pair of keys: a public key and a private key. The public key is used for encryption, while the private key is kept secret and used for decryption.

Here's a high-level overview of how RSA encryption works:

- Key Generation: The first step is to generate a public-private key pair. This involves selecting two large prime numbers, p and q, calculating their product n = p * q, and choosing an exponent e that is relatively prime to (p-1) * (q-1). The values of n and e make up the public key, while p, q, and a derived value d form the private key.

- Encryption: To encrypt a message m, the sender uses the recipient's public key (n, e) and applies the encryption formula: c = m^e (mod n). Here, c represents the ciphertext.

- Decryption: The recipient, in possession of the private key (d), can decrypt the ciphertext c using the decryption formula: m = c^d (mod n). This recovers the original message m.

The security of RSA relies on the computational difficulty of factoring large numbers. As long as the prime factors of the modulus n are kept secret, it is computationally infeasible to determine the private key from the public key.

RSA is widely used for secure communication, digital signatures, key exchange, and other cryptographic applications. However, the security of RSA relies on the size of the keys used. As computing power advances, longer key lengths are required to maintain adequate security.
