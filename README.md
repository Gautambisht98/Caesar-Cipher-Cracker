````markdown
# 🔐 Caesar Cipher Cracker

A simple web-based **Caesar Cipher brute-force cracker** that demonstrates how weak encryption can be broken by systematically trying all possible shifts.

The application takes an **already encrypted Caesar Cipher message**, tests shifts from `0–25`, and displays each decrypted result while checking whether the output is likely to be English.

---

## ✨ Features

- 🔐 Caesar Cipher decryption
- ⚔️ Brute-force attack simulation
- 🔄 Tests all possible Caesar Cipher shifts
- 🔍 Basic English-text detection
- 📊 Real-time attack progress
- 🔢 Total attempts counter
- ⏱️ Time elapsed tracking
- ⚡ Attempts-per-second calculation
- 🎯 Potential match detection
- 🎚️ Adjustable attack speed
- ▶️ Start/Stop attack controls
- 📱 Responsive web interface

---

## 🧠 How It Works

The Caesar Cipher encrypts text by shifting each letter by a fixed number of positions in the alphabet.

For example, using a shift of `3`:

```text
HELLO WORLD
     ↓
KHOOR ZRUOG
````

The cracker takes the encrypted message and tries every possible shift:

```text
Encrypted Message
        ↓
    Shift 0
        ↓
    Shift 1
        ↓
    Shift 2
        ↓
      ...
        ↓
    Shift 25
        ↓
Possible Plaintext
```

For example:

```text
Shift 0  → KHOOR ZRUOG
Shift 1  → JGNNQ YQTNF
Shift 2  → IFMMP XPME
Shift 3  → HELLO WORLD
...
Shift 25 → LIPPS ASVPH
```

Each result is analyzed using a basic English-language heuristic to identify outputs that may represent meaningful plaintext.

---

## 🔐 Caesar Cipher

The Caesar Cipher is a classical substitution cipher where every letter is shifted by a fixed number of positions.

For example:

```text
A → D
B → E
C → F
...
X → A
Y → B
Z → C
```

With a key of `3`:

```text
HELLO
  ↓
KHOOR
```

Because the Caesar Cipher has a very small key space, it is vulnerable to brute-force attacks.

---

## ⚔️ Brute-Force Attack

A brute-force attack attempts all possible keys until a meaningful result is found.

For the Caesar Cipher, there are only **25 meaningful non-zero shifts**, making exhaustive search extremely easy.

The application demonstrates this by automatically testing each shift and displaying the result.

---

## 🔍 English Text Detection

The application includes a simple heuristic to identify whether a decrypted message may be English.

It checks the generated text for:

* Common English words
* Alphabetic words
* Word length patterns

Example:

```text
KHOOR ZRUOG
        ↓
Try different shifts
        ↓
HELLO WORLD
        ↓
⚠️ Possible English text
```

This is an educational heuristic and is **not a complete cryptanalysis algorithm**.

---

## 📊 Attack Statistics

While the attack is running, the application displays:

| Statistic         | Description                       |
| ----------------- | --------------------------------- |
| Total Attempts    | Number of shifts tested           |
| Time Elapsed      | Time taken by the attack          |
| Attempts/Second   | Attack speed                      |
| Potential Matches | Results that may resemble English |
| Progress          | Percentage of shifts tested       |

---

## 🎚️ Attack Speed

The application provides a speed control that allows users to adjust the delay between attack attempts.

This makes it possible to:

* Slow down the attack for learning
* Observe each shift individually
* Demonstrate the brute-force process visually
* Speed up the simulation

---

## 🛠️ Technologies Used

* **HTML5** — Application structure
* **CSS3** — Interface and responsive design
* **JavaScript** — Cipher logic, brute-force attack, statistics, and UI interaction

No backend or database is required.

---

## 📁 Project Structure

```text
Caesar-Cipher-Cracker/
│
├── index.html
└── README.md
```

The complete application is currently implemented inside `index.html`.

---

## 🚀 How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/Gautambisht98/Caesar-Cipher-Cracker.git
```

### 2. Open the Project

```bash
cd Caesar-Cipher-Cracker
```

### 3. Run the Application

Open:

```text
index.html
```

in a modern web browser.

You can also open the project in **Visual Studio Code** and use the **Live Server** extension.

---

## 🧪 Example

### Input

```text
Encrypted Message:

KHOOR ZRUOG
```

### Brute-Force Process

The application attempts different shifts:

```text
Shift 0 → KHOOR ZRUOG
Shift 1 → JGNNQ YQTNF
Shift 2 → IFMMP XPME
Shift 3 → HELLO WORLD
...
```

The application highlights results that appear to be potential English text.

---

## 🎯 Project Objective

The main objective of this project is to demonstrate:

* How the Caesar Cipher works
* How classical encryption can be attacked
* How brute-force attacks work
* Why small key spaces are insecure
* How cryptanalysis can be implemented using JavaScript
* How an attack can be visualized through a web interface

---

## 📚 Learning Outcomes

This project provides practical understanding of:

* Classical cryptography
* Caesar Cipher encryption and decryption
* Brute-force attacks
* Cryptanalysis
* Key-space analysis
* JavaScript programming
* String manipulation
* DOM manipulation
* Event handling
* Real-time UI updates
* Basic English-text analysis

---

## ⏱️ Complexity

For a Caesar Cipher, the number of possible meaningful keys is constant:

```text
25 possible shifts
```

For a message of length `n`, testing every shift requires approximately:

```text
Time Complexity: O(25 × n)
```

Since `25` is a constant, this can effectively be considered:

```text
O(n)
```

for a fixed Caesar Cipher alphabet.

The important security point is that the **key space is extremely small**, making brute-force attacks practical.

---

## ⚠️ Limitations

* The project is designed primarily for educational purposes.
* English detection uses a simple heuristic.
* A potential match does not necessarily mean the result is the correct plaintext.
* The application only targets Caesar Cipher encryption.
* It does not implement modern cryptographic algorithms.
* It should not be used for protecting sensitive information.

---

## 🔒 Security Disclaimer

This project is intended for **educational and cybersecurity learning purposes only**.

The Caesar Cipher is a classical cipher and is **not secure for modern communication**.

Use this tool only with messages or systems that you own or have permission to analyze.

---

## 🔮 Future Improvements

Possible future improvements include:

* Automatic best-key selection
* Frequency-analysis-based cryptanalysis
* Dictionary-based plaintext scoring
* Support for multiple classical ciphers
* Encryption and decryption modes
* Visual alphabet-shift demonstration
* Attack-result ranking
* Performance comparison between different cracking techniques
* Dark mode
* Improved mobile interface
* Detailed attack logs

---

## 🎓 Project Category

**Cybersecurity / Cryptography / Web Development**

This project can be used as an educational demonstration of **classical cryptography and brute-force cryptanalysis**.

---

## 👨‍💻 Author

**Gautam Bisht**

GitHub: [@Gautambisht98](https://github.com/Gautambisht98)

---

## ⭐ Support

If you found this project useful for learning **cryptography and cybersecurity concepts**, consider giving the repository a ⭐.

```
```
