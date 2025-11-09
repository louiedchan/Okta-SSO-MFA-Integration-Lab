# Okta-SSO-MFA-Integration-Lab
Hands-on lab demonstrating Okta Single Sign-On (SSO), Multi-Factor Authentication (MFA), and user lifecycle management in a free Okta Developer environment.


# 🔐 Okta SSO & MFA Integration Lab

## 🧩 Overview
This lab demonstrates how to configure **Okta Single Sign-On (SSO)**, **Multi-Factor Authentication (MFA)**, and **User Lifecycle Management** in a free **Okta Developer** environment.  
The goal is to simulate how an **IAM Engineer** would securely integrate Okta with cloud or SaaS applications, enforce MFA, and manage user access — all while following best practices for identity governance.

---

## 🎯 Objectives
- Configure a free Okta Developer tenant  
- Create and manage user accounts  
- Enable MFA (Okta Verify & Email)  
- Integrate an AWS or custom sandbox app for SSO  
- Test and validate least-privilege access controls  
- Deactivate users to demonstrate lifecycle management  

---

## 🧰 Tools & Technologies
| Tool | Purpose |
|------|----------|
| **Okta Developer Console** | Identity Provider configuration |
| **Okta Verify App** | MFA factor |
| **AWS Sandbox / Custom OIDC App** | SSO target |
| **Browser / Incognito Mode** | Testing user experience |
| **GitHub** | Documentation & version control |

---

## 🪜 Step-by-Step Implementation

### **Phase 1 — Environment & Directory Setup**
1. Dashboard or Getting Started screen showing my name and tenant ID in the top-right corner.
![User List](./screenshots/Screenshot%202025-11-08%20154748.png)
2. Create Users
3. 
### **Phase 2 — SAML + SSO Integration**
1.

📸 **Screenshot #2:** Student LabUser details screen.

---

### **Step 3 — Enable MFA**
1. Navigate to **Security → Multifactor**.  
2. Enable **Okta Verify** and **Email**.  
3. Set MFA required for all users under **Security → Authentication → Sign-On Policy**.

📸 **Screenshot #3:** MFA policies showing Okta Verify & Email enabled.

---

### **Step 4 — Integrate an App for SSO**
Option A — AWS App Integration  
1. Go to **Applications → Browse App Catalog → Search “Amazon Web Services”**.  
2. Add integration and assign to Student LabUser.  

Option B — Custom Web App (OIDC)  
1. Click **Create App Integration → OIDC – OpenID Connect → Web**.  
2. Assign it to Student LabUser.

📸 **Screenshot #4:** AWS or Custom App added and assigned.

---

### **Step 5 — Test SSO & MFA**
1. Open a new browser/incognito tab.  
2. Go to your Okta tenant URL.  
3. Log in as `Student LabUser`.  
4. Complete MFA enrollment and test login to the app.  

📸 **Screenshot #5:** MFA prompt.  
📸 **Screenshot #6:** Successful SSO dashboard with app tile.

---

### **Step 6 — Deactivate the User**
1. Back in Admin Console: **Directory → People → Student LabUser → Deactivate**.  
2. Confirm user status = “Deactivated”.

📸 **Screenshot #7:** Deactivated user record.

---

### **Step 7 — Clean Up**
- Review MFA and SSO configurations.  
- Remove test apps and users.  
- Sign out of all sessions.

📸 **Screenshot #8:** Final Okta dashboard after cleanup.

---

## 📂 Folder Structure Example
