
# 🔐 Domain 1.2: Non-repudiation

---

## 1️⃣ Foundations of Cryptography in Verification 🧩

**Key Concept:** Cryptography isn’t just about hiding data—it’s also about proving who sent it and that it hasn’t been altered.

**Non-repudiation**  
Ensures that a sender cannot deny sending data.  
**Analogy:** Signing a paper contract. Anyone can check the signature later and confirm the sender.

Two main components of non-repudiation:

- **Proof of Integrity** – The data received is exactly the data sent. ✅  
- **Proof of Origin** – The sender of the data can be verified. 📨

---

## 2️⃣ Proof of Integrity 🔑

**Definition:** Confirms that the content of the data has not been altered during transmission.

**How it works:**  
Use a hash function:  
- A hash is a short, unique string of text derived from the original data.  
- Also called: **message digest** or **fingerprint**.  
- Even a tiny change in the original data results in a completely different hash.

**Real-world Example:**  
1. Download Project Gutenberg Encyclopedia Volume 1 (8.1 MB).  
2. Generate a hash for the file.  
3. Modify even one character.  
4. Generate a new hash → It will be different.  
5. Comparison shows that the file has been altered.

**Key takeaway:** Hashes prove data integrity, but **do not identify the sender**. 🕵️‍♂️

---

## 3️⃣ Proof of Origin / Authentication ✍️

**Definition:** Confirms who sent the data.

**Digital Signatures**  
- Provide non-repudiation and proof of origin.  
- **Analogy:** Just like signing a contract but digitally.  

**How digital signatures work:**

1. Sender (Alice) has a **private key** (known only to her). 🔒  
2. Hash the plaintext message (e.g., "You're hired, Bob."). #️⃣  
3. Encrypt the hash with Alice's private key → becomes the **digital signature**.  
4. Send the plaintext + digital signature to the recipient (Bob). 📨

**Verification by recipient (Bob):**  
1. Bob receives the message + signature.  
2. Bob uses Alice's **public key** (available to anyone) to decrypt signature. 🔑  
3. Bob now has the original hash created by Alice.  
4. Bob hashes the plaintext message he received.  
5. Compare the two hashes:  
   - **Match** → Message is intact and from Alice ✅  
   - **Mismatch** → Message was altered or not from Alice ⚠️

**Key Points:**  
- Digital signatures rely on **asymmetric cryptography** (private/public key pair).  
- Usually happens automatically (e.g., click "Add digital signature").  

---

## 4️⃣ Step-by-Step Digital Signature Process 📝

| Step | Action | Purpose |
|------|--------|---------|
| 1 | Sender creates hash of message | Proof of integrity |
| 2 | Sender encrypts hash with private key | Creates digital signature (proof of origin) |
| 3 | Sender sends message + signature | Transmit securely |
| 4 | Receiver decrypts signature with sender's public key | Retrieve original hash |
| 5 | Receiver hashes received message | Generate local hash |
| 6 | Compare hashes | Confirm integrity and authenticity |

**Mnemonic to remember:**  
**H-E-S-H-C → Hash, Encrypt, Send, Hash, Compare** 🔄

---

## 5️⃣ Key Concepts Summary 📚

- **Hash Function:** Verifies data integrity. #️⃣  
- **Digital Signature:** Verifies both integrity and origin. ✍️  
- **Non-repudiation:** Prevents sender from denying their message. 🧾  
- **Private Key:** Used to sign/encrypt the hash. 🔒  
- **Public Key:** Used to verify signature. 🔑  
- **Proof of Integrity:** Message unchanged. ✅  
- **Proof of Origin:** Message came from the claimed sender. 📨

---

## 6️⃣ Quick Analogies / Memory Anchors 🧠

- 📝 **Contract Signature Analogy:** Paper contract ↔ Digital signature  
- 🔑 **Keys Analogy:** Private key = secret pen; Public key = magnifying glass to check pen marks  
- 🕵️‍♂️ **Fingerprint Analogy:** Hash = unique fingerprint of data; tiny change = different fingerprint  

---

## 7️⃣ Flashcards for Active Recall 🎴

**Q:** What is non-repudiation in cryptography?  
**A:** Assurance that the sender cannot deny sending the data.

**Q:** What does a hash function provide?  
**A:** Proof of integrity; detects if data has changed.

**Q:** Can a hash function identify the sender?  
**A:** No, it only verifies data integrity.

**Q:** What is a digital signature?  
**A:** Encrypted hash of a message using the sender’s private key; proves integrity + origin.

**Q:** How does the recipient verify a digital signature?  
**A:** Decrypts with sender’s public key and compares hashes.

**Q:** What’s the difference between proof of integrity and proof of origin?  
**A:** Integrity = message unchanged; Origin = message from the claimed sender.

---

## ✅ Takeaway

By understanding **hashes** and **digital signatures**, you can ensure that data is **unchanged** and truly from the **claimed sender**, essential for secure communications, contracts, and cryptographic transactions. 🔐
