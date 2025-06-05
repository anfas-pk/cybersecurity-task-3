# 🔒 Task 3 - Basic Vulnerability Scan (Cybersecurity Internship)

## 📌 Objective
Perform a basic vulnerability assessment on my local machine using **Nessus Essentials** to identify and understand common security risks.

---

## 🛠️ Tool Used
- **Nessus Essentials** (by Tenable)
- Scan Type: *Basic Network Scan*
- Target: *Localhost (192.168.56.1)*

---

## 🧪 Scan Summary
- **Scan Start**: 4:01 PM  
- **Scan End**: 4:08 PM  
- **Elapsed Time**: 8 minutes  
- **Vulnerabilities Found**: 23

---

## 📊 Vulnerability Breakdown
| Severity | Count |
|----------|-------|
| 🟠 Medium | 1     |
| 🟪 Mixed  | 1     |
| 🔵 Info   | 21    |

---

## ⚠️ Notable Findings

### 1. **SMB Signing Not Required** (Medium Severity)
- **CVSS Score**: 5.3
- **Risk**: Leaves the system vulnerable to *man-in-the-middle (MITM)* attacks.
- **Mitigation**: Enable SMB signing via Windows group policy or registry settings.

### 2. **SSL / TLS Issues** (Mixed Severity)
- Multiple issues found in:
  - **SSL Configuration**
  - **TLS Weak Ciphers**
- **Impact**: May allow downgrade attacks or traffic decryption.
- **Fix**: Enforce modern cipher suites and disable legacy protocols.

---

## 📁 Included in Repository
- 📸 `screenshots/` folder (Nessus scan results)
- 📝 `README.md` (this file)

---

## 📚 Concepts Learned
- Vulnerability scanning vs. penetration testing
- CVSS scoring system
- Importance of regular vulnerability assessments
- Mitigation strategies for common findings

---

---

> ✅ **Next Steps**: Patch medium-severity issues, disable weak SSL/TLS configs, and schedule periodic scans for improved security posture.
