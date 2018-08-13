# LinuxONE-modprobe

The	Linux	kernel	implements	a	set	of	cryptographic	mechanisms: hashes	and	symmetric	crypto,	pseudo	random	numbers.

The Kernel	architecture	allows	to	replace	software	implementation	by	hardware implementations in	a	modular	manner.
Modular modules being:
* sha_common
* sha1_s390
* sha256_s390
* sha512_s390
* ghash_s390
* aes_s390
* prng
* ctr
* xts
* gcm
* hmac

## modprobe about ciphers
```
modprobe aes_s390     # to support AES ciphers hardware acceleration
modprobe des_s390     # to support DES and 3DES ciphers hardware acceleration
```

## modprobe about digests
```
modprobe sha_common   # to support SHA relative digests with the hardware
modprobe sha1_s390    # to support SHA1 ciphers with the hardware
modprobe sha256_s390  # to support SHA2-256, SHA2-224  ciphers with the hardware
modprobe sha512_s390  # to support SHA2-512, SHA2-384 ciphers with the hardware
```

## modprobe about other functions
```
modprobe rng          # to support random number generation with the hardware  
modprobe prng         # to support pseudo-random number generation with the hardware
modprobe ghash        # to support GHASH with the hardware
modprobe hmac         # to support hash Message Authenticated Code with the hardware
```

## modprobe about hardware and adjunc processors
```
modprobe ap           # to support Adjuncted Processors
modprobe z90crypt     # to support z90crypt defice driver to find and attach crypto cards hardware
```

## modprobe about mode of operation
```
modprobe gcm          # to support GCM mode of operation with the hardware  
modprobe xts          # to support XTS mode of operation with the hardware  
```
