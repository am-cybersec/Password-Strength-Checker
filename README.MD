# Password Strength Analyzer

A Python tool that demonstrates how weak passwords are cracked using **dictionary attacks** and **brute-force attacks** — built to show why strong passwords matter in cybersecurity.

## 🎯 What It Does

Tests password strength by simulating real attack techniques used by hackers:

1. **Dictionary Attack** — tries common passwords from a wordlist first
2. **Brute Force Attack** — systematically tries all character combinations if dictionary fails

## 🔐 How It Works

```
Target Password → SHA-256 Hash → Attack Simulation → Result
```

| Attack Type | Method | Speed |
|---|---|---|
| Dictionary | Common wordlist | Very Fast |
| Brute Force | All combinations | Depends on length |

## 🛠️ Tech Stack

- Python 3
- `itertools` — combination generation
- `hashlib` — SHA-256 hashing
- `string` — character sets
- `time` — performance tracking

## 🚀 How to Run

```bash
# Clone repo
git clone https://github.com/am-cybersec/Password-Strength-Analyzer

# Run
python password_analyzer.py
```

## 📊 Sample Output

```
Trying dictionary attack...
Dictionary attack failed. Falling back to brute force (max length 4)...
[Brute Force] Password found: mimi
Attempts: 45832 | Time: 2.4531 sec
```

## ⚙️ Customize

```python
# Add your own wordlist
wordlist = ["admin", "password", "123456", "yourword"]

# Set target password to test
test_password = "your_password_here"

# Set max brute force length
MAX_BRUTE_LENGTH = 4
```

## 💡 Key Concepts Demonstrated

- SHA-256 password hashing
- Dictionary attack simulation
- Brute force attack with itertools
- Attack performance measurement
- Why short/common passwords are dangerous

## 🔑 Security Lesson

| Password | Attack Success | Time |
|---|---|---|
| `admin` | Dictionary ✅ | < 1ms |
| `mimi` | Brute Force ✅ | ~2 sec |
| `X9#mK2$pL` | Both ❌ | Years |

**Strong passwords = longer crack time = better security**

## 📸 Output Screenshot

![Password Analyzer Output](screenshot.png)

## 🎓 Project Context

| Detail | Info |
|---|---|
| Course | Design & Analysis of Algorithms |
| Institution | COMSATS University Islamabad |
| Topic | Cybersecurity / Password Security |