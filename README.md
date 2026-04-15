📝 Soroban Smart Notes App
📖 Application Description
Soroban Smart Notes is a decentralized CRUD (Create, Read, Update, Delete) application built natively on the Stellar network using the Soroban smart contract ecosystem. Designed as a capstone project for the Rise In: Build on Stellar Bootcamp - Telkom University, this application allows users to securely create, read, modify, and delete personal notes immutably stored on the blockchain.

By moving away from basic workshop examples, this contract demonstrates a fundamental understanding of Soroban's state management, custom struct definitions, and deterministic pseudo-random number generation (PRNG) for unique record identification.

✨ Core Features
Create Note: Generates a new note with a secure, auto-generated random ID using Soroban's native PRNG (env.prng().gen()) and stores it on the ledger.

Read Notes: Retrieves all existing notes stored within the contract's instance storage seamlessly.

Update Note: Allows modification of an existing note's title and content by finding its specific ID and updating the storage state.

Delete Note: Enables the removal of a specific note from the blockchain using its unique ID, preventing ledger bloat.

🔗 Smart Contract Deployment Details
The smart contract binaries were developed using the soroban.studio cloud IDE, optimized for the WebAssembly target, and successfully deployed to the Stellar Testnet infrastructure.

Network Environment: Stellar Testnet (Test SDF Network ; September 2015)

Smart Contract ID: <YOUR_CONTRACT_ID_HERE> (e.g., C...)

Deployer Account: <YOUR_SOURCE_ACCOUNT_ADDRESS_HERE>

💻 Testnet Execution & CLI UI Screenshot
(The following screenshot demonstrates the operational state verification and state mutations via the Stellar CLI remote procedure call interface executed directly from a Linux bash terminal on soroban.studio).

!(./assets/screenshot.png)

(Note for the Developer before committing: Execute a successful stellar contract invoke command traversing the CRUD functions on your soroban.studio terminal, take a clear screenshot of the output, and save it exactly as screenshot.png inside an assets/ subdirectory).

🛠️ Build & Deployment Instructions (Linux / soroban.studio environment)
1. Toolchain Prerequisites
Ensure the environment possesses the correct Rust compiler target and the unified Stellar CLI:

Bash
rustup target add wasm32-unknown-unknown
cargo install --locked stellar-cli --features opt
2. Contract Compilation & Optimization
Bash
stellar contract build
3. Execution & Deployment to Testnet
Bash
stellar contract deploy \
  --wasm target/wasm32-unknown-unknown/release/notes_contract.wasm \
  --source-account <your_funded_account> \
  --network testnet
