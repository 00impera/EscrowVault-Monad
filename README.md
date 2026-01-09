<p align="center">
  <img src="NEW_LOGO_URL" alt="Dragon Escrow Vault Logo" width="120" />
</p>

<h1 align="center">Dragon Escrow Vault</h1>

<p align="center">
  <b>Secure, upgradeable, profit-generating escrow smart contract for Monad</b><br>
  <i>Digital, cosmic-green, and user-friendly escrow platform</i>
</p>

---

## 📝 Project Description

**Dragon Escrow Vault** is an upgradeable, secure escrow smart contract system for the Monad blockchain.  
It enables buyers and sellers to transact safely with an optional arbiter, platform fee, and a modern digital dashboard.  
The platform is designed for transparency, security, and ease of use, with a beautiful cosmic-green UI.

---

## 🏦 Features

- **Escrow creation** with buyer, seller, and optional arbiter
- **2% platform fee** (configurable by owner)
- **Dispute resolution** and refunds
- **Upgradeable (UUPS)** for future improvements
- **Owner controls:** pause, unpause, update fee, emergency withdraw
- **Digital, cosmic-green dashboard UI** (HTML/JS, no build step)
- **Secure:** ReentrancyGuard, Pausable, Ownable (OpenZeppelin)

---

## 📁 Directory Structure

dragon-escrow-vault/ ├── src/ │ └── DragonEscrowVault.sol # Main escrow contract ├── script/ │ └── Deploy.s.sol # Foundry deployment script ├── frontend/ │ └── index.html # Digital dashboard UI ├── foundry.toml # Foundry config ├── .env.example # Example environment variables ├── README.md # Project documentation └── ... # (other files as needed)

---

## 🔒 Contract Files

- **src/DragonEscrowVault.sol**  
  Main upgradeable escrow contract (UUPS, Ownable, Pausable, ReentrancyGuard, 2% platform fee).

- **script/Deploy.s.sol**  
  Foundry deployment script for proxy pattern.

---

## 🚀 How to Use

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/dragon-escrow-vault.git
cd dragon-escrow-vault

2. Install dependencies
forge install

3. Configure environment
Copy .env.example to .env and fill in your secrets:
PRIVATE_KEY=your_private_key
MONAD_RPC_URL=https://monad-mainnet.g.alchemy.com/v2/your-alchemy-key
MONAD_BLOCKVISION=https://monad-mainnet.blockvision.org/v1/your-blockvision-key
FEE_COLLECTOR=your_fee_collector_address

4. Deploy contract
source .env
forge script script/Deploy.s.sol:DeployDragonEscrow --rpc-url $MONAD_RPC_URL --private-key $PRIVATE_KEY --broadcast -vvvv

5. Run the frontend
Open frontend/index.html in your browser.
Connect your wallet and interact with the escrow dashboard.
📜 Example Contract Address
0x39B0A759C18B50ab4126a94dF1B86947BB51a6e4
View on Monad Explorer

🛡️ Security
Uses OpenZeppelin upgradeable contracts
ReentrancyGuard, Pausable, Ownable
No private keys or secrets in repo
Platform fee is capped (max 10%)
🤝 License
MIT

🐉 Credits
Built by the DRAGON Team 🚀
Logo: Pinata IPFS
