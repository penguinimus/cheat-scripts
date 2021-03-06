Cryptography
============

Stream Cipher: bits of data encrypted in a continious stream, fast, XOR

#### Symmetric  algorithms

Symmetric Encryption: single key, shared key. one key used to encrypt / decrypt
 
	DES       # 56 bit key, 8 bit parity (obsolete)
	3DES	  # 168 bit key, uses up to 3 keys
	AES       # 128, 192 or 256 bit keys, block cipher
	IDEA      # 128 bit key
	Twofish   # 265 bit key, block cipher
	Blowfish  # 32 to 448 bit key, 64 bit block size, block cipher
	RC6       # up to 2040 bit keys, 128 bit key blocks, block cipher 

#### Asymmetric algorithms

Asymmetric Encryption: key pair generated together. public key encrypts, private key decrypts

	Diffie-Hellman   # Key exchange protocol, SSL, IPSec 
	ECC              # Eliptic curve, encryption and digital signatures
	El Gamal         # encryption and digital signatures
	RSA              # standard for encryption and digital signatures

#### Hash algorithms:

Hash algorithm: one way function, takes an input and produces a string (hash)  
hashes are susceptible to collisions, two or more files resulting in same hash output  
Salt: collection of random bits used as a key with hash.

	MD5       # 128 bit output as a 32 digit hex (obsolete)
	SHA-1     # 160 bit output (obsolete)
	SHA-2     # 224, 256, 384, 512 bit output 


#### PKI System

Framework for key distribution


Trust Model:

	Web of trust                # multiple entities sign certificates for one another
	Single authority system     # CA at the top that issues certs
	Hierarchical trust system   # CA at top with intermediate CA's underneath (RA's)

X.509 Standard for Digital Certificates:

	Version
	Serial Number
	Subject
	Signature Algorithm
	Issuer
	Valid From and Valid To
	Key Usage
	Subject's Public Key
	Optional Fields

Encryption of digital cert is done with private key, public key used to verify authenticity 


#### Attacks

Known plaintext attack: attacker has both plaintext and ciphertext and scans for repeatable sequences  
Chosen plaintext attack: attacker encrypts multiple plaintext copies to gain the key  
Ciphertext only attack: has serveral copies of message encrypted in same way, finds repeating code  
Replay attack: Done with MITM, repeats portions of message back to system to trick it into communicating  



