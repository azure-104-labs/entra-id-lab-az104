# entra-id-lab-az104
Hands-on lab for managing identities using Microsoft Entra ID (Azure AD), covering user/group creation, guest users, and Microsoft 365 &amp; Security groups. Part of the AZ-104 study series focused on building a solid foundation in Azure administration.

# Azure AD (Entra ID) Lab — Section 3: Users, Groups & Devices

This repository documents my hands-on lab work while preparing for the **Microsoft Azure Administrator (AZ-104)** exam.  
Section 3 covers identity-centric tasks in **Microsoft Entra ID (formerly Azure AD)**.

---

## 1. Users

| Type | Count | Notes |
|------|-------|-------|
| Internal | **18** | Distributed across HR, IT, Claims, Finance, Client Services |
| External/Guest | **3** | Invited via Azure AD B2B collaboration |

> Each user received a unique UPN and was placed into at least one group as part of RBAC planning.

---

## 2. Groups

### Microsoft 365 Groups  
- Enable collaboration in Outlook, SharePoint, Teams.  
- Assigned to users who need productivity services.

### Security Groups  
- Control access, device policies, license assignment.  
- **Owned by IT** for centralized governance.

> **Next step:** evaluate *function-* or *role-based* grouping to tighten RBAC & Conditional Access.

---

## 3. Administrative Units (AUs)

| Status | Notes |
|--------|-------|
| ⚠️ Created | Full delegation blocked—requires **Azure AD Premium P2** (trial activation pending) |

---

## 4. License Assignment

- **Direct:** a few test users.  
- **Group-based:** primary method for scalability.

---

## 5. Device Management

| Item | Details |
|------|---------|
| Hypervisor | VirtualBox |
| Devices | Local VMs (Win 10/11) |
| Join Type | Azure AD Join / Hybrid Join |
| Verified Properties | Name, OS, Trust Type, Join Date |
| Group Membership | Added to appropriate security groups |
| Licensing | Microsoft 365 applied where applicable |

---

## Screenshots

Below are selected visuals from the lab.  
*(See all in `/images` folder.)*

## Screenshots

Here are selected visuals that show the real progress and configuration inside my Azure AD lab.  
*(See all in `/images` folder.)*

| No. | Filename         | Description |
|-----|------------------|-------------|
| 1   | (./images/1.png.png) | **VMs Setup** – VirtualBox machines created for lab testing |
| 2   | `2.png`          | **Azure VM Join** – VM successfully joined to Azure AD (Entra ID) |
| 3   | `3.png`          | **VM Details** – System and device information from the Azure portal |
| 4   | `4.png`          | **Directory Stats** – Overview of users, devices, and groups |
| 5   | `5.png`          | **User Accounts** – List of created internal and external users |
| 6   | `6.png`          | **Device Joined** – Confirmation of VM joined status in Entra ID |
| 7   | `7.png`          | **User Profile** – Properties and group membership of a specific user |
| 8   | `8.png`          | **Password Reset** – Self-service or admin-based reset UI example |
| 9   | `9.png`          | **Entra Connect** – Connector details or sync setup (if applicable) |
| 10  | `10.png`         | **Group Management** – Microsoft 365 and Security group structure |


---

## What’s Next

- Deep-dive into **RBAC**  
- Build **Conditional Access** policies  
- Finish P2 trial activation to fully test AUs  
- Continue recording notes & scripts (PowerShell) in upcoming sections

---

> **Feedback / PRs welcome!**  
> If you have suggestions on group strategy or P2 trial activation, please open an issue or reach out.
