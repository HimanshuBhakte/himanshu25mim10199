# 🔐 Password Helper

> *Because "password123" is basically an open door.*

```
██████╗  █████╗ ███████╗███████╗██╗    ██╗ ██████╗ ██████╗ ██████╗ 
██╔══██╗██╔══██╗██╔════╝██╔════╝██║    ██║██╔═══██╗██╔══██╗██╔══██╗
██████╔╝███████║███████╗███████╗██║ █╗ ██║██║   ██║██████╔╝██║  ██║
██╔═══╝ ██╔══██║╚════██║╚════██║██║███╗██║██║   ██║██╔══██╗██║  ██║
██║     ██║  ██║███████║███████║╚███╔███╔╝╚██████╔╝██║  ██║██████╔╝
╚═╝     ╚═╝  ╚═╝╚══════╝╚══════╝ ╚══╝╚══╝  ╚═════╝ ╚═╝  ╚═╝╚═════╝ 
                                                        H E L P E R
```

---

## 🧐 What is this?

A simple, no-nonsense **command-line password tool** built in Python. It does two things really well:

- 🔍 **Checks** if your password is strong enough to survive the real world
- ⚙️ **Generates** a strong random password when you can't be bothered to think of one

---

## ✨ Features

| Feature | Description |
|---|---|
| 🧪 Password Checker | Instantly tells you what's wrong with your password |
| 🎲 Password Generator | Creates a random 8-character strong password |
| 💡 Helpful Tips | Gives you advice when your password is weak |
| 🖥️ Simple Menu | Clean 3-option interface — no fluff |

---

## 🚀 Getting Started

### Prerequisites

Just Python 3! No external libraries needed.

```bash
python --version  # Make sure you have Python 3.x
```

### Run It

```bash
python password_helper.py
```

You'll see this friendly menu:

```
=== Password Helper ===
1. Check my password
2. Make strong password
3. exit

Choose 1, 2 or 3:
```

---

## 🎮 How to Use

### Option 1 — Check My Password

Enter any password and get instant feedback:

```
Choose 1, 2 or 3: 1
Enter password to check: hello

Weak: Too short! Use at least 8 characters

How to make strong:
- Use 8+ characters
- Mix UPPERCASE and lowercase
- Add numbers like 123
- Add symbols like !@#
- Example: Vasco&burn67
```

### Option 2 — Generate a Strong Password

Let the tool do the work:

```
Choose 1, 2 or 3: 2

New password: kR3!mXpQ
This has all needed: letters, CAPS, numbers, symbols!
```

### Option 3 — Exit

```
Choose 1, 2 or 3: 3

Tata and Bye-Bye! 👋
```

---

## 🛡️ What Makes a Password "Strong"?

The checker validates **5 rules** — all must pass:

```
✅  At least 8 characters long
✅  Contains UPPERCASE letters  (A–Z)
✅  Contains lowercase letters  (a–z)
✅  Contains numbers            (0–9)
✅  Contains symbols            (!@#$%&*)
```

Fail even one? It tells you exactly which rule you broke.

---

## 🏗️ How It Works (Under the Hood)

```
password_helper.py
│
├── check_password(password)
│   └── Validates against 5 rules one by one
│       and returns a "Weak: ..." or "Strong: ..." message
│
└── make_password()
    ├── Picks 1 char from each required category
    │   (lowercase, UPPERCASE, number, symbol)
    ├── Adds 4 more random characters from the full set
    └── Shuffles everything for randomness
```

---

## 🧩 Symbols Supported

The tool recognises these special characters:

```
! @ # $ % & *
```

---

## 📁 Project Structure

```
password-helper/
└── password_helper.py   # The whole project — one clean file!
```

---

## 💡 Example Strong Passwords

These would all pass the checker:

```
Vasco&burn67
X9#mPqLw
Hello@99
Sun$et12
```

---

## 🔮 Ideas for Future Upgrades

- [ ] Add a password strength **score** (0–100)
- [ ] Support **longer** generated passwords
- [ ] Add a **clipboard copy** feature
- [ ] Check passwords against a list of common ones
- [ ] Build a simple **GUI** with Tkinter

---

## 👨‍💻 Author

Built with ❤️ and Python.  
*Stay safe. Use strong passwords. Don't recycle them.*

---

## 📜 License

Free to use, share, and improve. Just don't use it to generate weak passwords on purpose. 😄
