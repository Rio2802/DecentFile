📄 Blockchain-Based Document Storage with IPFS

A secure, decentralized, and tamper-proof system for storing and verifying documents using Blockchain and IPFS (InterPlanetary File System).
This project ensures document integrity by storing files on IPFS and recording their immutable hashes on the blockchain.

✅ Overview

This system provides a reliable approach for storing sensitive documents in a decentralized environment.
Instead of storing documents directly on the blockchain (which is expensive and inefficient), files are uploaded to IPFS, and only the file hash is saved on the blockchain.

This ensures:

🔐 Integrity — A document cannot be modified without changing its hash.

🌍 Decentralization — No single point of failure.

⚡ Fast Retrieval — Documents load quickly from the distributed IPFS network.

✅ Trustless Verification — Anyone can verify authenticity without needing permission.

✨ Features

🔒 Secure Document Storage using IPFS + Blockchain

🌐 Fully Decentralized Architecture

⚡ Fast Document Upload/Retrieval

🧩 Supports Multiple File Formats

👨‍💻 User-Friendly Web Interface

✅ Automatic Hash Recording on Blockchain

📦 Requirements

Before running the project, ensure you have:

Node.js & npm

MetaMask Wallet (browser extension)

IPFS API credentials
→ You can generate them from Infura or Pinata

Smart contract deployed using Remix IDE

🛠️ Installation & Setup
1️⃣ Install dependencies
npm install

2️⃣ Deploy Smart Contract

Open Remix IDE

Load and deploy contract.sol

Copy the deployed contract address

3️⃣ Configure the Frontend

Paste the contract address into app.js

Configure:

Network RPC URL

Network Explorer URL
(Available in MetaMask custom network settings)

4️⃣ Add IPFS Credentials

Inside uploadToInfura function in app.js, paste your:

IPFS API Key

IPFS API Secret

5️⃣ Run the Application

Use Live Server:

Right-click index.html → "Open with Live Server"


Your DApp is now running locally!

🚀 Usage Guide
✅ Add an Exporter

Click Add Exporter

Enter the MetaMask address of the exporter

✅ Upload a Document

Click Upload Document

Select any file

The file is:

Uploaded to IPFS

Returned with a unique IPFS hash

Hash is stored on the Blockchain

✅ Retrieve a Document

Click Retrieve Document

Enter the document’s hash

The file is automatically fetched from IPFS and displayed

📁 Project Architecture
Frontend (HTML/JS)
     │
     ├── Interacts with MetaMask
     ├── Uploads files → IPFS (Infura)
     │
Smart Contract (Solidity)
     │
     └── Stores IPFS Hashes on Blockchain

🛡️ Security Benefits

✅ Tamper-proof document storage

✅ No central authority

✅ Verifiable document integrity

✅ Resistant to server failures

📜 License

This project is licensed.
Feel free to use, modify, and enhance.
