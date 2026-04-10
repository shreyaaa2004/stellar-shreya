# Stellar Payment Tracker

A blockchain-based invoice and payment management system built on the **Stellar Soroban** network. Track invoices, manage payments, and handle overdue accounts seamlessly on-chain.

## 📸 Screenshots

### Landing Page
![Landing Page](https://raw.githubusercontent.com/shreyaaa2004/stellar-shreya/main/docs/landing-page.png)
Beautiful welcome screen with project overview and "Get Started" button to enter the application.

### Main Application Interface
![Main Application](https://raw.githubusercontent.com/shreyaaa2004/stellar-shreya/main/docs/app-interface.png)
Connected wallet status, tabbed navigation for invoice creation, payment actions, and queries with real-time blockchain integration.

### Smart Contract on Stellar Expert
![Contract Explorer](https://raw.githubusercontent.com/shreyaaa2004/stellar-shreya/main/docs/contract-explorer.png)
View contract details, transaction history, and on-chain data on Stellar Expert blockchain explorer.

## 🎯 Features

- **Create Invoices**: Generate unique invoices with issuer, recipient, and payment details
- **Mark Payments**: Record paid invoices with payment amounts and timestamps
- **Track Overdue**: Automatically flag overdue invoices
- **Cancel Invoices**: Revoke invoices when needed
- **Query Invoices**: Lookup individual invoices or list all invoices
- **Outstanding Balance**: Calculate total outstanding payments
- **Wallet Integration**: Connect your Freighter wallet for blockchain transactions
- **Real-time Blockchain**: All transactions are recorded on Stellar Soroban

## 🚀 Getting Started

### Prerequisites
- Node.js (v16 or higher)
- npm or yarn
- [Freighter Wallet](https://www.freighter.app/) extension installed

### Installation

```bash
# Clone the repository
git clone https://github.com/shreyaaa2004/stellar-shreya.git
cd stellar-shreya

# Install dependencies
npm install

# Start the development server
npm run dev
```

The app will be available at `http://localhost:5174/`

## 📋 Usage

### 1. Landing Page
- Beautiful landing page with project overview
- Click "Get Started" to enter the application
- Responsive design for all devices

### 2. Connect Wallet
- Click "Connect Freighter" to link your Stellar wallet
- Shows connected wallet address and status
- Wallet remains connected during your session

### 3. Create Invoice
- Navigate to "Create Invoice" tab
- Fill in invoice details:
  - Invoice ID (unique identifier)
  - Issuer & Recipient addresses
  - Description & Amount
  - Due date (Unix timestamp)
- Click "Create Invoice" to submit to blockchain

### 4. Payment Actions
- Mark invoices as paid with payment amount and date
- Flag invoices as overdue
- Cancel invoices with confirmation

### 5. Queries & Reports
- Lookup specific invoices
- View all invoices
- Get total outstanding balance

## 🏗️ Architecture

```
src/
├── App.jsx                 # Main application component
├── App.css                 # Styling
└── lib/
    └── stellar.js          # Stellar Soroban integration
```

### Landing Page Component
- Welcoming UI with project description
- Smooth transition to main application
- Responsive and accessible design

### Main Application
- Tab-based navigation (Create, Payment, Queries)
- Real-time wallet connection status
- Transaction logging and output display
- Connected wallet display at top

## 🔗 Blockchain Integration

Uses **Stellar Soroban** for:
- Immutable invoice storage
- Secure payment tracking
- On-chain verification
- Smart contract execution

### Contract Details

**Smart Contract Address:**
```
CC5XU2ZPWISYJC7KO5MONDNLO6V2XLZJCME5PGKD3RUTZBSRJNNVV5PT
```

**View on Stellar Expert:**
[Contract Explorer - CC5XU2ZPWISYJC7KO5MONDNLO6V2XLZJCME5PGKD3RUTZBSRJNNVV5PT](https://stellar.expert/explorer/testnet/contract/CC5XU2ZPWISYJC7KO5MONDNLO6V2XLZJCME5PGKD3RUTZBSRJNNVV5PT)

**Contract Information:**
- Created: 2026-04-10 06:20:28 UTC
- Type: WASM Contract
- Network: Testnet
- Creator: GCI4...QWMJ
- Hash: 6b61c957...a147510a

## 🎨 UI Features

- **Landing Page**: Beautiful gradient background with hero section
- **Responsive Design**: Works on desktop, tablet, and mobile
- **Dark Theme**: Easy on the eyes with green accents
- **Loading States**: Visual feedback during transactions
- **Status Indicators**: Real-time wallet and transaction status
- **Tab Navigation**: Clean interface for different operations
- **Transaction Output**: Real-time logging of all blockchain actions

## 📝 Form Validation

All inputs are validated before submission:
- Invoice IDs (max 32 characters)
- Valid Stellar addresses (G...)
- Proper timestamp formats (Unix seconds)
- Amount validation (numeric values)
- Required field checks

## ⚙️ Environment Setup

Create a `.env` file in the root directory:

```env
VITE_SOROBAN_RPC_URL=https://soroban-testnet.stellar.org
VITE_NETWORK_PASSPHRASE=Test SDF Network ; September 2015
VITE_CONTRACT_ID=CC5XU2ZPWISYJC7KO5MONDNLO6V2XLZJCME5PGKD3RUTZBSRJNNVV5PT
```

## 🧪 Transaction Log

Every action is logged with:
- Transaction status (success/error)
- Response data in JSON format
- Timestamp of execution
- Clear error messages for debugging
- Contract invocation details

## 🔐 Security

- Private keys never leave your wallet
- All transactions require wallet approval
- Uses Freighter for secure key management
- On-chain verification for all operations
- No sensitive data stored locally

## 📦 Dependencies

- React 18+
- Vite (build tool)
- Stellar JS SDK
- Soroban SDK
- Freighter API

## 🐛 Troubleshooting

### Wallet not connecting?
- Ensure Freighter extension is installed
- Check if you're on a supported network
- Try refreshing the page
- Check browser console for errors

### Transaction failing?
- Verify you have enough XLM for fees
- Check address format (must start with G)
- Review the transaction log for error details
- Ensure due date is in future timestamp

### Contract not found?
- Ensure you're on the Testnet
- Verify contract ID: `CC5XU2ZPWISYJC7KO5MONDNLO6V2XLZJCME5PGKD3RUTZBSRJNNVV5PT`
- Check [Stellar Expert](https://stellar.expert/explorer/testnet/contract/CC5XU2ZPWISYJC7KO5MONDNLO6V2XLZJCME5PGKD3RUTZBSRJNNVV5PT)
- Verify RPC URL is correct

## 📄 License

MIT License - feel free to use this project for personal or commercial purposes.

## 👤 Author

**Shreya**
- GitHub: [@shreyaaa2004](https://github.com/shreyaaa2004)
- Project: Stellar Payment Tracker

## 🙏 Acknowledgments

- Stellar Development Foundation
- Soroban documentation
- Freighter wallet team

---

**Built with ❤️ on the Stellar Blockchain**