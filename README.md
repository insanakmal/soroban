# Soroban Smart Notes 📝

A decentralized, on-chain note-taking application built on the **Stellar Testnet** using the **Soroban Smart Contract** framework. [cite_start]This project demonstrates a full CRUD (Create, Read, Update, Delete) cycle for managing persistent data on the blockchain. [cite: 66, 67]

## 📖 Description
[cite_start]**Soroban Smart Notes** is a smart contract designed to allow users to store personal notes securely on the Stellar network. [cite: 68] [cite_start]Each note is stored with a unique ID, a title, and content. [cite: 69] [cite_start]The contract handles state storage efficiently using Soroban's `instance` storage, ensuring that your data remains accessible and tamper-proof. [cite: 70]

## ✨ Key Features
* [cite_start]**Create Note:** Add new entries with a title and description. [cite: 71]
* [cite_start]**Get All Notes:** Retrieve the full list of stored notes in a structured format. [cite: 72]
* [cite_start]**Update & Delete:** Modify existing notes or remove them from the ledger using their unique IDs. [cite: 113]
* [cite_start]**Unique Identification:** Each note is automatically assigned a unique `u64` ID. [cite: 73]
* [cite_start]**Testnet Verified:** Fully deployed and tested using Stellar Laboratory and Soroban CLI. [cite: 74]

## 🔗 Deployment Details
* [cite_start]**Network:** Stellar Testnet [cite: 75]
* [cite_start]**Contract ID:** `CC2MXFL6AV4JN2M6KCKIAFBXGRE3TZ7AVPSKCG2JJMKQB3XLVKO5FIYP` [cite: 29, 75]
* [cite_start]**Wasm Hash:** `301d93b1a87e5ae4a104ee4b8e69731e7741a994fd5e660b48b6fc6953192a73` [cite: 75]

---

## 📸 Testnet Interaction (Screenshots)

### 1. Contract Deployment
[cite_start]The contract was successfully instantiated on the Stellar Testnet. [cite: 76]
![Contract Created](./screenshots/Screenshot_2026-04-16_130535.png)

### 2. Invoking `Notes`
[cite_start]Successful transaction adding the first note: **"FirstNote"**. [cite: 77]
> [cite_start]**Result:** "Notes berhasil ditambahkan" [cite: 78]
![Invoke Create Note](./screenshots/Screenshot_2026-04-16_130550.png)

### 3. Reading Data via `get_notes`
[cite_start]Querying the contract storage returns the stored note data in JSON format. [cite: 79]
![Read Notes](./screenshots/Screenshot_2026-04-16_130956.png)

---

## 🛠 Usage Guide

### Build
Compile the smart contract to WASM:
```bash
stellar contract build
[cite_start]
http://googleusercontent.com/immersive_entry_chip/0
http://googleusercontent.com/immersive_entry_chip/1
http://googleusercontent.com/immersive_entry_chip/2

### Panduan Tambahan:
1.  [cite_start]**Folder Gambar:** Buatlah folder bernama `screenshots` di repositori GitHub Anda. [cite: 80]
2.  [cite_start]**Unggah Screenshot:** Masukkan file gambar yang Anda miliki (misalnya `Screenshot 2026-04-16 130535.png`) ke dalam folder tersebut dan pastikan namanya sesuai dengan yang tertulis di file `README.md` di atas. [cite: 80]
3.  [cite_start]**Identitas Akun:** Jangan lupa untuk mengganti `YOUR_ACCOUNT_NAME` dengan nama identitas lokal Anda (seperti `release` atau `indramahesa`) saat menjalankan perintah terminal. [cite: 81]
