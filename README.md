# 🔐 Password Strength Analyser & Credential Breach Checker Tool

A web-based security tool that analyses the strength of a password and checks whether it has been exposed in known data breaches — built as part of the Rooman Technologies Internship (CS-EH Track).

---

## 📌 Features

- ✅ Real-time password strength analysis (Weak / Medium / Strong)
- ✅ Entropy-based scoring for accurate strength measurement
- ✅ Credential breach check using the [HaveIBeenPwned API](https://haveibeenpwned.com/API/v3)
- ✅ k-Anonymity model — your password is **never sent** to any server
- ✅ Remediation advice and security recommendations based on results
- ✅ Clean, single-file HTML tool — no installation needed

---

## 🚀 How to Use

1. Download or clone this repository
2. Open `index.html` in any web browser
3. Enter a password in the input field
4. View the strength score, breach status, and security recommendations instantly


---

## 🛡️ How the Breach Check Works (k-Anonymity)

This tool uses the **HaveIBeenPwned Pwned Passwords API** with k-Anonymity:

1. Your password is hashed using **SHA-1**
2. Only the **first 5 characters** of the hash are sent to the API
3. The API returns a list of matching hash suffixes
4. The tool checks locally if your full hash is in that list
5. **Your actual password never leaves your browser**

---

## 📁 Project Structure

```
📦 password-strength-checker
 ┗ 📄 index.html       # Main tool (all-in-one HTML file)
 ┗ 📄 README.md        # Project documentation
```

---

## 🔧 Technologies Used

- HTML, CSS, JavaScript (Vanilla)
- HaveIBeenPwned Pwned Passwords API
- SHA-1 hashing (Web Crypto API)
- Entropy-based password scoring

---



## 👨‍💻 Author

**Sudeep**
Intern — Cyber Security & Ethical Hacking Track
Rooman Technologies

---

## 📜 License

This project is for educational purposes as part of an internship program.
