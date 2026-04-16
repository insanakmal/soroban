Soroban Smart Notes 📝
A decentralized, on-chain note-taking application built on the Stellar Testnet using the Soroban Smart Contract framework. This project demonstrates a full CRUD (Create, Read, Update, Delete) cycle for managing persistent data on the blockchain.

📖 Description
Soroban Smart Notes is a smart contract designed to allow users to store personal notes securely on the Stellar network. Each note is stored with a unique ID, a title, and content. The contract handles state storage efficiently using Soroban's instance storage, ensuring that your data remains accessible and tamper-proof.

✨ Key Features
Create Note: Add new entries with a title and description.

Get All Notes: Retrieve the full list of stored notes in a structured format.

Unique Identification: Each note is automatically assigned a unique u64 ID.

Testnet Verified: Fully deployed and tested using Stellar Laboratory and Soroban CLI.

🔗 Deployment Details
Network: Stellar Testnet

Contract ID: CC2MXFL6AV4JN2M6KCKIAFBXGRE3TZ7AVPSKCG2JJMKQB3XLVKO5FIYP

Wasm Hash: 301d93b1a87e5ae4a104ee4b8e69731e7741a994fd5e660b48b6fc6953192a73

📸 Testnet Interaction (Screenshots)
1. Contract Deployment
The contract was successfully instantiated on the Testnet.

(Note: Use your 'Screenshot 2026-04-16 130535.png' here)

2. Invoking Notes
Successful transaction adding the first note: "FirstNote".

Result: "Notes berhasil ditambahkan"

(Note: Use your 'Screenshot 2026-04-16 130550.png' here)

3. Reading Data via get_notes
Querying the contract storage returns the note data in JSON format.

(Note: Use your 'Screenshot 2026-04-16 130956.png' here)

🛠 Usage Guide
Build
Bash
stellar contract build
Deploy
Bash
stellar contract deploy \
  --wasm target/wasm32-unknown-unknown/release/notes.wasm \
  --source-account YOUR_ACCOUNT \
  --network testnet
Create a Note
Bash
stellar contract invoke \
  --id CC2MXFL6AV4JN2M6KCKIAFBXGRE3TZ7AVPSKCG2JJMKQB3XLVKO5FIYP \
  --source-account YOUR_ACCOUNT \
  --network testnet \
  -- create_note --title "My Title" --content "Hello World"
🏗 Technology Stack
Language: Rust

Platform: Soroban Smart Contracts

Network: Stellar Testnet

Tools: Soroban CLI, Stellar Laboratory
