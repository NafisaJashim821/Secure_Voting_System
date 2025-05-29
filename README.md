# Secure Voting System

A simple **Java-based command-line application** that simulates a secure voting process using **RSA encryption**. This project is designed to ensure **vote confidentiality**, **voter authentication**, and **prevention of duplicate votes**.

## 🔐 Features

- **RSA Key Generation:** Dynamically generates public and private keys at runtime.
- **Secure Voting:** Votes are encrypted before being stored and decrypted only for result tallying.
- **User Authentication:** Only registered users (name and NID) can access the voting system.
- **One Vote per User:** The system ensures that each user can vote only once.
- **Time-restricted Voting:** Voting is allowed only between 8 AM and 4 PM.
- **Vote Result Display:** Total vote counts for each candidate are displayed securely.

  ## 📁 Project Structure

```
SecureVotingSystem/
│
├── SecureVotingSystem.java     # Entry point of the application
├── VotingManager.java          # Manages the voting session and user interface
├── VotingProcessor.java        # Handles encryption, decryption, vote recording
├── users.txt                   # Contains list of registered voters (name,NID)
├── encryptedVotes.txt          # Stores encrypted votes and NID
├── decryptedVotes.txt          # Stores decrypted votes for counting
└── README.md                   # Project overview and usage
```

## 🔄 Clone the Repository

To get a local copy of this project, run the following command:

```bash
git clone https://github.com/NafisaJashim821/Secure_Voting_System.git

## 🗳️ Voting Interface

1. Log in using your name and NID (must be listed in `users.txt`).
2. Cast your vote by choosing one of the available candidates.
3. After voting, you can:
   - View results
   - Exit the system

