# 🔐 1.2: AAA, Authentication, Authorization, and Accounting

---

## 1️⃣ AAA Framework 🔑

AAA = Authentication, Authorization, Accounting

**Authentication** – Confirms that you are who you claim to be.  
Example: Username + password + additional factors (MFA).  
Methods include:
- Passwords 🔒  
- Biometric factors 👤  
- Digital certificates (for devices) 💻  

**Authorization** – Determines what access you have once authenticated.  
Example: A shipping employee can access shipping systems but not finance systems.  

**Accounting** – Logs actions for auditing and security. 📊  
Tracks login times, resource usage, and logout events.  

**Key takeaway:** AAA ensures secure access and accountability across systems. ✅

---

## 2️⃣ Authentication Process 🔐

**Step 1: Identification**  
User claims an identity (e.g., entering username).  

**Step 2: Authentication**  
System checks credentials (password, token, certificate).  
Confirms identity matches the claim.  

**Example: Logging in to a VPN 🌐**

- User provides username and password 🔑  
- VPN concentrator forwards credentials to AAA server  
- AAA server validates credentials against central database 🗄️  
- VPN concentrator allows access if credentials are valid ✅  

---

## 3️⃣ Device Authentication Using Certificates 💻📜

**Problem:** How to verify that a computer/device is authorized without a password?  

**Solution:** Digital Certificates  

- **Certificate:** Digital credential installed on device 📄  
- **Certificate Authority (CA):** Trusted entity that issues and signs certificates 🏢  

**Process:**
1. Create a certificate for a device (e.g., company laptop) 💻  
2. CA digitally signs the certificate ✍️  
3. Install certificate on the device  
4. During authentication, the system checks the device certificate against the CA 🔍  

**Result:** Confirms the device is company-owned and trusted ✅  

**Key points:**

- Device certificate validates identity without storing passwords on the device 🔐  
- CA may itself be signed by a root CA for trust in the infrastructure 🌐  

---

## 4️⃣ Authorization Models 👥

**Purpose:** Determines access rights efficiently, especially in large organizations.  

**Challenges without an authorization model:**
- Assigning rights and permissions individually for each user is not scalable ❌  

**Example:**  
100 shipping employees need access to 50 resources → 5000 manual permission assignments 😵  

---

### Scalable Solution: Authorization Models / Abstraction ⚙️

- Group users into roles (e.g., "Shipping & Receiving") 👥  
- Assign permissions to the group once 🔑  
- Add users to the group → automatically inherits permissions ✅  

**Example:**

- Resources: Create shipping label, track shipments, view reports, customer data 📦  
- Group: Shipping & Receiving 👥  
- Users: Add all employees → automatic access to resources  

**Benefit:** Efficiently scales for hundreds or thousands of users 🚀  

---

## 5️⃣ Key Takeaways 📌

- AAA framework ensures secure, authorized, and auditable access 🔐  
- Authentication: Confirms identity (user/device) 👤  
- Authorization: Determines access to resources 🔑  
- Accounting: Logs activity for auditing 📊  
- Certificates + CA: Enable device authentication and trust 🌐  
- Authorization models: Abstract users from resources for easier management ⚙️  

---

## 6️⃣ Analogies / Memory Anchors 🧠

🔑 **AAA analogy:**
- Authentication = proving your ID at the door 🪪  
- Authorization = deciding which rooms you can enter 🚪  
- Accounting = recording when you came and left 📝  

💻 **Device certificate analogy:**  
Laptop has a “digital badge” signed by HQ (CA) to prove it belongs 🏢  

👥 **Group authorization analogy:**  
Giving access to a group instead of each person individually = adding all employees to a team with shared keys 🔑  

---

## 7️⃣ Flashcards for Active Recall 🎴

**Q:** What does AAA stand for in security?  
**A:** Authentication, Authorization, Accounting  

**Q:** What is authentication?  
**A:** The process of verifying a user/device is who they claim to be  

**Q:** What is authorization?  
**A:** Determining what resources a user/device can access after authentication  

**Q:** Why are certificates used in authentication?  
**A:** To verify devices are authorized without storing passwords on them  

**Q:** What is a Certificate Authority (CA)?  
**A:** A trusted entity that issues and signs digital certificates  

**Q:** How do authorization models help with scalability?  
**A:** By assigning permissions to groups/roles instead of individual users  

**Q:** Why is accounting important in AAA?  
**A:** To log and audit access, actions, and usage for security tracking  
