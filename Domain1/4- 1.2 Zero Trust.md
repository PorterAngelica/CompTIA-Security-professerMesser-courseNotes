---

# 🔐 1.2: Zero Trust

---

## 1️⃣ What is Zero Trust?

**Definition:**
A **Zero Trust network** assumes **nothing inside or outside the network is trusted** by default. Every access request must be verified.

**Key Principles:**

* Authenticate every user, device, and process **every time** they access a resource
* Apply security checks to **all devices, processes, and users**
* Minimize trust zones → security is **granular and continuous**

---

## 2️⃣ Why Traditional Networks Are Vulnerable

* Inside the firewall, networks are often **“flat”** → users can move freely
* Few internal controls → allows both:

  * Authorized users
  * Malicious actors or malware

**Zero Trust solves this** by requiring verification at **every step**.

---

## 3️⃣ Core Zero Trust Controls

1. **Multi-Factor Authentication (MFA)**
2. **Encryption**

   * Data at rest
   * Data in transit
3. **Permissions & Access Controls**
4. **Additional firewalls or segmentation**
5. **Policy-driven access**

---

## 4️⃣ Functional Planes in Security Devices

Security devices are split into **planes of operation**:

### 🖥️ Data Plane

* Performs **actual traffic handling**
* Examples: Forwarding packets, NAT, routing
* Real-time processing of data

### ⚙️ Control Plane

* **Manages the device** and policies
* Configures rules, routing, firewall policies
* Sets how the data plane operates

**Visualization:**

* Physical/virtual switches & firewalls → Data plane moves traffic, Control plane configures rules
* Cloud security → same concept applies

---

## 5️⃣ Adaptive Identity in Zero Trust

**Goal:** Strengthen authentication dynamically.

* Examine **identity + context**:

  * User’s location
  * Device type
  * IP address
  * Relationship to organization (employee, contractor, etc.)
  * Connection type (VPN, internal network, etc.)

* Systems can **automatically adjust authentication** based on risk

  * Example: User requests access from China → require MFA again

---

## 6️⃣ Security Zones

* Networks are segmented into **zones**:

  * Trusted, internal, external, untrusted, corporate offices, data centers, etc.
* Access rules depend on **source zone → destination zone**
* Can create:

  * **Implicit trust**: internal zones may have easier access
  * **Strict policies**: untrusted zones blocked by default

---

## 7️⃣ Policy-Based Access Control Model

Zero Trust uses **policy enforcement and decision separation**:

| Component                          | Role                                                           |
| ---------------------------------- | -------------------------------------------------------------- |
| **Policy Enforcement Point (PEP)** | Gatekeeper; traffic passes through, collects info              |
| **Policy Decision Point (PDP)**    | Makes decisions based on predefined policies                   |
| **Policy Engine**                  | Evaluates requests against rules; grants/denies/revokes access |
| **Policy Administrator**           | Communicates PDP decisions to PEP; issues tokens/credentials   |

**Flow:**

1. User/device request → PEP
2. PEP sends info → Policy Engine via Policy Administrator
3. Policy Engine decides → Administrator returns decision → PEP enforces

---

## 8️⃣ Putting It All Together: Zero Trust Workflow

1. Subject (user, device, process) requests access from **untrusted zone**
2. Data passes over **data plane**
3. Traffic reaches **Policy Enforcement Point** (gatekeeper)
4. Policy Engine checks policies → Policy Administrator communicates decision
5. PEP grants or denies access
6. If allowed → access to trusted zone/resource

**Key Concept:** Verification is **continuous, dynamic, and context-aware**.

---

## 9️⃣ Memory Anchors

* 🏰 **“Castle without a moat” → Zero Trust:** don’t trust anyone, even inside
* 🔄 **Adaptive authentication:** like a security alarm that changes sensitivity depending on threat
* 🛂 **Zones = check points:** each area has its own rules
* 👮 **PEP = gatekeeper, PDP = judge, Admin = messenger**

---

## 🔟 Flashcards (Active Recall)

1. **Q:** What is the principle of Zero Trust?
   **A:** Never trust by default; authenticate all users, devices, and processes continuously.

2. **Q:** Name the two planes in a security device.
   **A:** Data plane (handles traffic) and Control plane (manages policies/configuration).

3. **Q:** What is adaptive identity?
   **A:** Dynamically strengthening authentication using context like location, IP, device, and relationship.

4. **Q:** What is a Policy Enforcement Point (PEP)?
   **A:** The gatekeeper that intercepts requests and enforces policy decisions.

5. **Q:** What is the role of the Policy Decision Point (PDP)?
   **A:** Makes decisions on whether traffic should be allowed, denied, or revoked.

6. **Q:** How do security zones help in Zero Trust?
   **A:** They define rules for communication between different parts of the network.

7. **Q:** What is the overall flow of Zero Trust access control?
   **A:** Request → PEP → PDP/Engine → Admin → PEP → Access granted/denied.

---



Do you want me to do that next?
