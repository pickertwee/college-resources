# 🔐 Labwork 3: Cryptographic Operations using OpenSSL [Walkthrough](Walkthrough.md)

## A. Lab Objectives

This lab introduces you to **OpenSSL**, the GOAT of crypto toolkits, to vibe with:

- 🔒 Symmetric encryption (AES)
- 🔑 Asymmetric encryption (RSA)
- 🧩 Hashing (SHA-256)
- 🖋️ Digital signatures (RSA + SHA-256)

**By the end, you’ll flex your skills to:**
- Encrypt and decrypt files with AES and RSA.
- Generate and verify file hashes for data integrity.
- Create and verify digital signatures for authenticity.

---

## B. Lab Tasks

You gotta research and find the correct OpenSSL commands yourself — no hand-holding here. 😤

---

### Task 1: Symmetric Encryption and Decryption (AES-256-CBC)

**Scenario:**  
Labu wants to send a secret message to Labi. You’re about to encrypt it using AES-256-CBC — classic, but not bulletproof.

> 🔥 **Security Note:**  
> CBC mode? Meh. Vulnerable to padding oracle attacks. We’re just using it here ‘cause it’s simple. Real ops should use AES-256-GCM.

**Steps:**
1. Find how to generate a strong random key with `openssl rand`.
2. Write a message into a text file (e.g., `<YourName>.txt`).
3. Research `openssl enc -aes-256-cbc` to encrypt it.
4. Find out how to decrypt it back.
5. Compare original and decrypted content — they better match.

**Deliverables:**
- 📸 Screenshot of encryption & decryption commands.
- 📄 Show the original and decrypted file content side-by-side.

---

### Task 2: Asymmetric Encryption and Decryption (RSA)

**Scenario:**  
Labi wants messages encrypted with his **public key** only he can unlock with his **private key**.

> 🔥 **Security Note:**  
> RSA keys smaller than 2048 bits? That’s baby food. Only 2048+ allowed here.

**Steps:**
1. Research how to generate a 2048-bit RSA private key with `openssl genrsa`.
2. Extract the matching public key with `openssl rsa`.
3. Encrypt a file (`rahsia.txt`) using the **public key**.
4. Decrypt it using the **private key**.
5. Check that decrypted text = original secret sauce.

**Deliverables:**
- 📸 Screenshot of key generation, encryption, decryption.
- 📄 Original vs decrypted message proof.

---

### Task 3: Hashing and Message Integrity (SHA-256)

**Scenario:**  
Labu wants to make sure a doc wasn’t messed with. Enter: **SHA-256** hashing magic.

**Steps:**
1. Create a file (`<YourName>.txt`) with some random deep thoughts or whatever.
2. Hash it using `openssl dgst -sha256`.
3. Edit the file — just change a letter or emoji.
4. Hash it again.
5. Compare both hashes — spoiler alert: they gonna be different.

> ✨ **Alternative Tools:**  
> You *can* try `sha256sum`, but `openssl dgst` is your main star. If you do both, bonus points if you explain differences.

**Deliverables:**
- 📸 Screenshot of hashes before and after change.
- 🧠 Write a short explanation: why hashes flip out after small edits?

---

### Task 4: Digital Signatures using RSA

**Scenario:**  
Labu needs to digitally sign her doc (`agreement.txt`) to prove she’s the real MVP.

**Steps:**
1. Use the RSA private key you made in Task 2.
2. Create a text file (`agreement.txt`) you wanna sign.
3. Research how to sign it using `openssl dgst -sha256 -sign`.
4. Verify the signature with `openssl dgst -sha256 -verify`.
5. Modify `agreement.txt`, then try verifying again. Watch it flop.

**Deliverables:**
- 📸 Screenshot of signature creation and verification.
- 🧠 Explain why verification fails after tampering.

---

## C. Analyze Problems Encountered

Nobody gets it perfect first try. 😮‍💨 Spill the tea:

- Any syntax errors? Command oopsies?
- Confused by OpenSSL flags?
- File path dramas?
- Which error messages popped off?
- How did you debug and fix? (Google-fu, `man` pages, asking ChatGPT?)

Write down:
- What went wrong
- What you tried
- What finally worked
- Which resources you used

---

> 💬 **Tip:** Own your mistakes. It’s part of the glow-up. 🚀
  

