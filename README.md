# Electronic Voting System with XOR Encryption

A Python-based electronic voting system featuring XOR encryption and custom hash integrity verification.

---

## 📖 Description

This project was developed as part of a Supervised Practical Activity (APS) for the **Introduction to Structured Programming** course. The goal is to implement an electronic voting system capable of registering votes, encrypting data using XOR, and ensuring file integrity through a custom hash function built with Python's `os` library.

A second program will be developed to securely validate and tally the votes.

---

## 📦 Project Structure

### Program 1: Vote Registration, Encryption & Hash Generation
- Registers votes for different candidates
- Encrypts vote data using XOR with a fixed key
- Generates a custom hash of the encrypted data using the `os` library to ensure integrity
- Saves the encrypted votes and hash to a text file

### Program 2 *(to be implemented)*: Validation, Decryption & Tallying
- Validates the file based on the generated hash
- Decrypts the votes
- Tallies and displays the final results

---

## ✅ Prerequisites

- Python 3.x installed
- Python standard `os` library (no extra installs needed)

---

## 🚀 How to Run Program 1

**1. Clone the repository:**
```bash
git clone <repository_url>
cd <project_directory>
```

**2. Run the main program:**
```bash
python programa_urna.py
```

**3. Follow the terminal prompts:**
- Enter candidate names and vote counts
- Type `fim` when done to finish registration

**4. Check the generated file:**  
The program will save `votos_criptografados.txt` containing the encrypted votes and the generated hash. This file will be used by Program 2 for validation and tallying.

---

## 📄 Output File: `votos_criptografados.txt`

This file contains:
1. The encrypted vote data
2. The hash value generated with `os`, used to verify data integrity in Program 2

**Example output:**
```
ÊëÜé:1ÍÝãÜÜÜñ:2îòñññç,
f4a2d3e9b7a5f948a19c471c
```
- **Line 1**: Encrypted data
- **Line 2**: Hash of the encrypted data

---

## 🗂️ File Structure

```
├── programa_urna.py          # Program 1: registers, encrypts, and generates hash
├── votos_criptografados.txt  # Output file with encrypted votes and hash
└── README.md                 # This file
```

---

## 🛡️ License

This project is open source and available under the [MIT License](LICENSE).
