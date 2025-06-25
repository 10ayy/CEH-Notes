# Day 25 – Module 20: Cryptography

## 🔐 What is Cryptography?
Cryptography is the science of securing data by transforming it into an unreadable format to prevent unauthorized access. It ensures **confidentiality**, **integrity**, **authentication**, and **non-repudiation**.

---

## 🧾 Key Terminologies:
- **Plaintext** – The original readable data/message.
- **Ciphertext** – The encrypted form of the data.
- **Encryption** – The process of converting plaintext into ciphertext.
- **Decryption** – Converting ciphertext back into plaintext.
- **Algorithm** – The mathematical function used for encryption and decryption.
- **Key** – A string of bits used by cryptographic algorithms to alter data.

---

## 🧱 Types of Cryptography:

### 1. Symmetric Cryptography:
- Uses the **same key** for both encryption and decryption.
- **Algorithms**:  
  - DES (Data Encryption Standard)  
  - 3DES (Triple DES)  
  - AES (Advanced Encryption Standard)

### 2. Asymmetric Cryptography:
- Uses **two keys**: a **public key** for encryption and a **private key** for decryption.
- **Algorithms**:  
  - RSA (Rivest–Shamir–Adleman)  
  - DSA (Digital Signature Algorithm)

---

## 🧮 What is a Cipher?
A cipher is an algorithm used to perform encryption or decryption.

### 🔢 Types of Ciphers:
- **Caesar Cipher** – Shifts characters by a fixed number.
- **Substitution Cipher** – Replaces each character with another based on a mapping.
- **Transposition Cipher** – Rearranges the order of characters.

---

## 🔁 Encoding vs Encryption vs Hashing:
| Feature        | Encoding           | Encryption           | Hashing                  |
|----------------|--------------------|-----------------------|---------------------------|
| Purpose        | Data formatting    | Confidentiality       | Data integrity & storage |
| Reversible     | Yes                | Yes (with key)        | No                       |
| Example        | Base64             | AES, RSA              | MD5, SHA-1               |

---

## 🛡️ Applications of Cryptography:
- Secure communications (e.g., SSL/TLS)
- Digital signatures
- File encryption and secure backups
- Secure authentication (e.g., OTP, tokens)
- Blockchain and cryptocurrency

---

## 🧾 What is Hashing?
Hashing is the process of generating a fixed-length output (hash value) from an input string.

### 🔐 Hashing Algorithms:
- **MD5 (Message Digest 5)**
- **SHA-1 (Secure Hash Algorithm 1)**

### 🔑 What is Salting?
Salting is the technique of adding random data to the input of a hash function to prevent dictionary and rainbow table attacks.

### 🧰 Hashing Tools:
- `md5sum`, `hashcalc`, `cyberchef`, `base64.com`
- `crackthestation.net` (online hash analysis)

---

## 🔍 Applications of Hashing:
- Password storage and verification
- File integrity checks
- Digital signatures
- Blockchain

---

## 🖼️ What is Steganography?
Steganography is the practice of **concealing data within another medium**, such as images, audio, or video, to hide its existence.

### 🧭 Types of Steganography:
- **Image-based**
- **Audio-based**
- **Text-based**
- **Video-based**

### 🧪 Steganography Tools:
- `steghide`
- `stegcracker`
- `stegosuite`
- `quick stago`
- `deepsound`

---

## 📝 Summary:

On **Day 25**, I studied **Module 20: Cryptography**, covering the foundational concepts of **encryption, hashing, and steganography**. Key differences between **encoding, encryption, and hashing** were clarified, and popular algorithms and tools were introduced. This module reinforces the core principles of **data confidentiality, integrity, and concealment**, which are crucial for digital forensics, cybersecurity, and ethical hacking.

---
