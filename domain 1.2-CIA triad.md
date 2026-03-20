# 📘 Security+ SY0-701 Study Guide

## Domain 1.2 – The CIA Triad

---

## 1. Course Notes (Simple / Messer Style)

### What is the CIA Triad

The CIA Triad is the foundation of cybersecurity.

It defines the three main goals of security:

- Confidentiality  
- Integrity  
- Availability  

### Simple way to remember it
> CIA = what we are trying to protect

---

## Confidentiality

Confidentiality means keeping data private and preventing unauthorized access.

Only authorized users should see the data.

### Simple way to remember it
> Confidentiality = keep data secret

### Examples
- Encryption  
- Passwords  
- Access control  
- File permissions  

### Example
A company encrypts customer data so attackers cannot read it.  
👉 This protects **confidentiality**

---

## Integrity

Integrity means ensuring data is accurate and has not been altered.

Data should not be modified without authorization.

### Simple way to remember it
> Integrity = data is correct and unchanged

### Examples
- Hashing  
- Digital signatures  
- File integrity monitoring  

### Example
A system detects that a file was modified unexpectedly.  
👉 This protects **integrity**

---

## Availability

Availability means systems and data are accessible when needed.

Users should be able to access resources without interruption.

### Simple way to remember it
> Availability = systems are up and working

### Examples
- Backups  
- Redundancy  
- Load balancing  
- Failover systems  

### Example
A website stays online even during high traffic.  
👉 This protects **availability**

---

## 🧠 Cheat Sheet (Full Domain 1.2)
| Concept         | Meaning                 | Memory Trick              |
|-----------------|------------------------|---------------------------|
| Confidentiality | Keep data secret       | “No unauthorized access”  |
| Integrity       | Data is accurate       | “No changes”              |
| Availability    | Systems are accessible | “Always up”               |


## 🧠 Flashcards – Domain 1.2 (Security Concepts)

### CIA Triad

**Flashcard 1**  
**Q:** What are the three components of the CIA Triad?  
**A:** Confidentiality, Integrity, Availability  

---

**Flashcard 2**  
**Q:** What does confidentiality protect?  
**A:** Prevents unauthorized access to data  

---

**Flashcard 3**  
**Q:** What does integrity ensure?  
**A:** Data is accurate and not modified  

---

**Flashcard 4**  
**Q:** What does availability ensure?  
**A:** Systems and data are accessible when needed  

---

**Flashcard 5**  
**Q:** Data was modified without authorization. Which CIA principle is affected?  
**A:** Integrity  

---

**Flashcard 6**  
**Q:** A system is unavailable due to an outage. Which CIA principle is affected?  
**A:** Availability  

---

**Flashcard 7**  
**Q:** Unauthorized users accessed sensitive data. Which CIA principle is affected?  
**A:** Confidentiality  

---

## 4. Exam Tips (VERY IMPORTANT)

### How CompTIA tests this

They give scenarios like:

- “Data was modified without authorization”  
  👉 **Answer: Integrity**

- “System is unavailable due to an outage”  
  👉 **Answer: Availability**

- “Unauthorized users accessed sensitive data”  
  👉 **Answer: Confidentiality**

---

## 🧠 Memory Trick (Lock It In)

- **C → Confidential = secret**  
- **I → Integrity = intact**  
- **A → Available = accessible**  

---
---

## Domain 1.2 – Non-Repudiation

---

## 1️⃣ Course Notes (Simple / Messer Style)

### What is Non-Repudiation

Non-repudiation ensures that someone cannot deny that they performed an action.

It provides proof of origin and integrity of data.

### Simple way to remember it
> Non-repudiation = you can’t deny it

---

### Why It Matters

Without non-repudiation:

- A user could say: “That wasn’t me”  
- A sender could deny sending a message  
- A transaction could be disputed  

👉 Non-repudiation provides **accountability**

---

## 2️⃣ How It Works

Non-repudiation is usually achieved using:

---

### 1. Digital Signatures

- Proves who sent the data  
- Uses cryptography  

👉 Like signing a contract digitally  

---

### 2. Hashing

- Creates a unique fingerprint of data  
- If data changes → hash changes  

👉 Used to verify integrity  

---

### 3. Public Key Cryptography

- Combines encryption + signatures  

Ensures:
- Authenticity  
- Integrity  
- Non-repudiation  

---

## 🧠 Key Idea (VERY IMPORTANT)

Non-repudiation actually combines:

- **Authentication → who sent it**  
- **Integrity → data not changed**  

👉 Together = **cannot deny action**

---

## 3️⃣ Real-World Example

Alice sends a signed email to Bob.

Bob can verify:

- It came from Alice  
- It was not modified  

👉 Alice **cannot deny sending it**

---

## 4️⃣ Cheat Sheet (Quick Review)

| Concept            | Meaning                         |
|-------------------|---------------------------------|
| Non-repudiation   | Cannot deny an action           |
| Digital signature | Proves sender                   |
| Hashing           | Verifies data integrity         |
| Public key crypto | Enables signatures              |

---

## 5️⃣ Flashcards

### Flashcard 1
**Q:** What is non-repudiation?  
**A:** Assurance that someone cannot deny their actions  

---

### Flashcard 2
**Q:** What does non-repudiation prove?  
**A:** Who sent the data and that it wasn’t changed  

---

### Flashcard 3
**Q:** What technology is commonly used for non-repudiation?  
**A:** Digital signatures  

---

### Flashcard 4
**Q:** What role does hashing play in non-repudiation?  
**A:** Verifies data integrity  

---

### Flashcard 5
**Q:** What happens if data changes after hashing?  
**A:** The hash value changes  

---

### Flashcard 6
**Q:** What type of cryptography is used in digital signatures?  
**A:** Public key cryptography  
---
## 6️⃣ Exam Tips (VERY IMPORTANT)

### How CompTIA tests this

They don’t ask:

> “What is non-repudiation?”

They ask scenario-based questions.

---

### Example 1

A user sends a digitally signed message and later denies sending it.  

👉 **Answer: Non-repudiation**

---

### Example 2

A system verifies that a file has not been altered.  

👉 **Answer: Integrity (NOT non-repudiation ⚠️)**

---

## 🔥 KEY TRAP

- **Hashing alone → Integrity**  
- **Digital signature → Non-repudiation**  

---

## 🧠 Memory Trick

- **Signature = proof = non-repudiation**  
- **Hash = integrity only**  

