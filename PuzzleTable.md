# Bitcoin Private Key Dataset (2015)

A curated dataset of known Bitcoin private keys and their associated wallet addresses from cryptographic challenges (circa 2015).  
**For educational/research purposes only**.

---

## 📋 Table of Contents
- [Project Description](#-project-description)
- [Dataset Overview](#-dataset-overview)
- [Key Explanations](#-key-explanations)
- [Disclaimer](#-disclaimer)
- [References](#-references)

---

## 🧩 Project Description
This repository documents **historically revealed Bitcoin private keys** from early cryptographic experiments (January 2015). These keys were part of mathematical challenges to demonstrate Bitcoin's security boundaries.

---

## 📊 Dataset Overview

| #  | Private Key (Hex)                            | Wallet Address                     | Upper Range Limit | Compressed Public Key (Hex)                     | Solved Date  |
|----|----------------------------------------------|------------------------------------|-------------------|-------------------------------------------------|--------------|
| 01 | `0000000000000000000000000000000000000000000000000000000000000001` | 1BgGZ9tcN4rm9KBzDn7KprQz87SZ26SAMH | 1                 | `0279be667ef9dcbbac55a06295ce870b07029bfcdb2dce28d959f2815b16f81798` | 2015-01-15   |
| 02 | `0000000000000000000000000000000000000000000000000000000000000003` | 1CUNEBjYrCn2y1SdiUMohaKUi4wpP326Lb | 3                 | `02f9308a019258c31049344f85f89d5229b531c845836f99b08601f113bce036f9` | 2015-01-15   |
| 03 | `0000000000000000000000000000000000000000000000000000000000000007` | 19ZewH8Kk1PDbSNdJ97FP4EiCjTRaZMZQA | 7                 | `025cbdf0646e5db4eaa398f365f2ea7a0e3d419b7e0330e39ce92bddedcac4f9bc` | 2015-01-15   |
| 04 | `0000000000000000000000000000000000000000000000000000000000000008` | 1EhqbyUMvvs7BfL8goY6qcPbD6YKfPqb7e | 15                | `022f01e5e15cca351daff3843fb70f3c2f0a1bdd05e5af888a67784ef3e10a2a01` | 2015-01-15   |
| 05 | `0000000000000000000000000000000000000000000000000000000000000015` | 1E6NuFjCi27W5zoXg8TRdcSRq84zJeBW3k | 31                | `02352bbf4a4cdd12564f93fa332ce333301d9ad40271f8107181340aef25be59d5` | 2015-01-??   |

---

## 🔑 Key Explanations
- **Private Key (Hex)**: 64-character hexadecimal representation of the ECDSA private key.
- **Wallet Address**: Legacy Bitcoin address (Base58Check encoding).
- **Upper Range Limit**: Maximum value of the brute-force search range used to find the key.
- **Compressed Public Key**: 33-byte SEC-compressed public key starting with `02`/`03`.
- **Solved Date**: Date the key was successfully calculated (YYYY-MM-DD).

---

## ⚠️ Disclaimer
1. **Educational Use Only**: This data is provided for research/analysis purposes.
2. **Illegal Activity**: Accessing wallets you don't own is prohibited by law.
3. **Security Context**: Modern Bitcoin security makes brute-force attacks mathematically impractical (as of 2023).

---

## 📚 References
- [BIP-32: Hierarchical Deterministic Wallets](https://github.com/bitcoin/bips/blob/master/bip-0032.mediawiki)
- [Bitcoin Address Format](https://en.bitcoin.it/wiki/Address)
- [SEC 2: Recommended Elliptic Curve Domain Parameters](http://www.secg.org/sec2-v2.pdf)
