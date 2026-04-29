# 🌐 UniGib Subnetting Tool
### **University of Gibraltar | Networks Module: CSS51504**

Welcome to the official **Subnetting Calculator**, a specialized web application developed for students enrolled in the **CSS51504 Networks** module at the University of Gibraltar. This tool is designed to simplify complex IPv4 calculations and provide a visual breakdown of address space.

**Deployment URL:** `https://ug-subnet-calculator.vercel.app/`

---

## 🎓 Academic Alignment: CompTIA Network+
This tool is built to align strictly with **CompTIA Network+ (N10-008/009)** standards. Mastery of these concepts is essential for the exam and the CSS51504 module:

*   **CIDR Notation:** Understanding `/nn` notation (Classless Inter-Domain Routing).
*   **IP Classes:** Identifying Class A, B, and C address boundaries.
*   **Binary Visualization:** Seeing how the subnet mask "masks" the host bits to create network segments.
*   **Special Cases:** Proper handling of RFC 3021 (31-bit prefixes) and host addresses (/32).

---

## 🛠 How Subnetting Works
Subnetting is the practice of dividing a single physical network into two or more logical sub-networks (subnets).

1.  **The Network ID:** The first address in a range. It identifies the "wire" and cannot be assigned to a host.
2.  **The Broadcast Address:** The last address in a range. Used to communicate with every host on that subnet.
3.  **The Subnet Mask:** A 32-bit filter. `1` bits belong to the **Network**; `0` bits belong to the **Host**.
4.  **The Usable Range:** Addresses between the Network ID and Broadcast. 
    *   *Formula:* $2^n - 2$ (where $n$ is the number of host bits).

---

## 📝 Subnetting Cheat Sheet


| CIDR | Subnet Mask | Total Hosts | Usable Hosts | Notes |
| :--- | :--- | :--- | :--- | :--- |
| **/32** | 255.255.255.255 | 1 | 1 | Single Host Route |
| **/30** | 255.255.255.252 | 4 | 2 | Standard Point-to-Point Link |
| **/29** | 255.255.255.248 | 8 | 6 | Small Office / DMZ |
| **/28** | 255.255.255.240 | 16 | 14 | Small Subnet |
| **/27** | 255.255.255.224 | 32 | 30 | Mid-size Subnet |
| **/24** | 255.255.255.0 | 256 | 254 | Standard Class C |
| **/16** | 255.255.0.0 | 65,536 | 65,534 | Standard Class B |
| **/8** | 255.0.0.0 | 16,777,216 | 16,777,214 | Standard Class A |

---

## 🚀 Features
*   **Real-time Calculations:** Network IDs, Broadcasts, and Host counts.
*   **Subnet Breakdown Table:** Break larger blocks into smaller segments (e.g., /24 into /30s).
*   **Binary Bit Grid:** Highlights the "Network vs. Host" bit boundary.
*   **Vercel Optimized:** Lightweight and accessible from any device.

---

## 📜 Licence
**Open Academic Licence (Free for All)**
This tool is provided as a free resource for students and educators. 
*   **Permitted Use:** Free to use, modify, and distribute for any purpose.
*   **Cost:** 100% Free.
*   **Attribution:** Mention of the **University of Gibraltar Networks Module** is appreciated.
*   https://opensource.org/license/AFL-3.0

---

## 👨‍🏫 For Students
Use this tool to verify your manual calculations during your lab sessions. **Note:** In the CSS51504 exam, you will need to perform these calculations manually; use this app to build your intuition.
