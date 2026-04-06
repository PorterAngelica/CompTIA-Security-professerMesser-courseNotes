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
# 1.2 The CIA Triad 🔐


## Confidentiality 🔒
If we want to prevent someone from gaining access to private information, we need to provide that information in a confidential way.  
Prevent disclosure of information to unauthorized individuals or systems.  

The biggest challenge we have in IT is making data available to others, but making sure that availability is only to the right people. We refer to this as confidentiality. One way we can provide this is through encryption.  

---

### Encryption 🔐
We can have one person encrypt data, send it to someone else, and that other person can decrypt that data to be able to see the original plaintext (message). Anyone in the middle who happens to get access to that encrypted data has no idea what’s on the inside. And if they were to look at that data, they would not be able to discern anything important from that information.  

Encode messages so only certain people can read it.  

---

Another way to provide confidentiality is to set limits on what someone may have access to. We commonly do this with access controls.  

---

### Access controls 🛂
We can limit who might have access to certain types of information. Ex: this might allow someone in the marketing department to be able to see all of the marketing presentations and be able to make changes to those. But it would prevent all access to any accounting information of the organization.  

Selectively restrict access to a resource.  

---

### Two-Factor authentication 🔑
If you ever need to provide additional authentication factors when logging into a system, that's another type of confidentiality. Someone would not be able to access an account unless they had the proper authentication credentials. And adding those additional factors provides more confidentiality.  

Additional confirmation before information is disclosed.  

---

## Integrity 🧩
Where, if  we are sending information from one person to another, we want to make sure the recipient really is receiving exactly what was sent from the originator  
Messages can’t be modified without detection  

When we are receiving data for a third party, we’d like to verify that the data we have received is exactly the same data that was sent and nobody has made changes to that data while it was traversing the network.  
Data is stored and transferred as intended  
Any modification to the data would be identified  

We are able to do that by using methods of integrity. One way to provide integrity is by hashing.  

---

### Hashing #️⃣
The person sending the data will create a hash of the data and send you both the data and the hash at the same time. When you receive the data, you’ll perform the same hashing function, and if your hash matches your sender’s hash, then you know that the data you’ve received is exactly the same data that was sent.  

Map data of an arbitrary length to data of a fixed length.  

---

We can enhance this integrity by including a digital signature.  

---

### Digital Signatures ✍️
When we’re sending data, which takes a hash and encrypt it with an asymmetric encryption algorithm. This means we can check to make sure none of the data has changed and we can confirm the person who sent the data, which also provides an additional level of integrity, and that could be important if you’re sending sensitive data.  

Mathematical scheme to verify the integrity of data.  

---

### Certificates 📜
It's common to use certificates to be able to identify devices or people and provide additional factors of integrity, especially when you are transferring data from one device to another.  

Combine with a digital signature to verify an individual.  

---

## Non-repudiation 🧾
This means we have proof of integrity, and we can confirm without a doubt that the information that we’ve received really did come from the originating party.  

Provides proof of integrity, can be asserted to be genuine.  

---

## Availability ⚡
We want to make sure that all of our systems remain up and running at all times.  

Availability ensures that people have access to the data that they’d like to view  
Systems and networks must be up and running.  

---

### Redundancy ♻️
one way to provide this availability is to have systems that are designed to be always up and running.  

Build services that will always be available.  

We might combine this with a system that has fault tolerance.  

---

### Fault tolerance ⚙️
Fault tolerance is where we have multiple components, and if one of those components fails, the other component picks up and continues to operate normally.  

The system will continue to run, even when a failure occurs.  

---

If you are concerned about systems being available, you’ll constantly need to make sure that they are managed and updated by patching those systems.  

---

### Patching 🔄
This ensures that the systems are always as stable as possible and that we can close any existing security holes, preventing someone from gaining access through some type of exploit.  

Stability  
Close security holes  

---



