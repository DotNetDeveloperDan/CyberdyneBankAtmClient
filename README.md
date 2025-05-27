# 🖥️ CyberdyneBankAtmClient

> The web ATM client for CyberdyneBankAtm — “Where your funds become self-aware.”

This is the **Blazor WebAssembly front-end** for the CyberdyneBankAtm application.  
It emulates an ATM user experience: deposit, withdraw, transfer, and view account history — all from your browser.

---

## 🚀 Features

- **ATM-style interface** built with Blazor WebAssembly (.NET 9)
- Interacts with the CyberdyneBankAtm API for all account actions
- Supports deposit, withdraw, and transfer operations
- View real-time account balances and transaction history
- Global, dismissible notifications for success and errors
- Responsive, touch-friendly, and simple by design

---

## 🏁 Getting Started

### Requirements

- [.NET 9 SDK](https://dotnet.microsoft.com/download/dotnet/9.0)
- The CyberdyneBankAtm backend API running (see its own README)

### 1. Run the API Server (if not already running)

```bash
cd ../CyberdyneBankAtm.Api
dotnet run
```
(Default: https://localhost:8081)

### 2. Run the Blazor Client

```bash
cd CyberdyneBankAtm.Client
dotnet run
```
(Default: https://localhost:7282)

### 3. Open in Browser

Go to [https://localhost:7282](https://localhost:7282)  
The app will auto-connect to the API (CORS must be enabled on the backend).

---

## 🖱️ Usage

- **Accounts Page:** View all accounts and balances (default landing page)
- **Account Details:** See transaction history for each account
- **Deposit/Withdraw:** Make deposits or withdrawals with ATM-style form
- **Transfer:** Move funds between Checking & Savings accounts
- **Notifications:** Popup messages for all operations

---

## ⚙️ Configuration

- API base URL is set in `Program.cs` via `HttpClient` registration.
- All CORS and API-side setup is handled in the backend.

---

## 🛠️ Extending

- Add new account or transaction views by editing the Razor pages in `/Pages`.
- Add more notification types or advanced UI in the `/Shared` and `/Services` folders.
- Connect to a different backend by changing the `BaseAddress` for `HttpClient`.

---

## 📄 License

MIT — for demo and educational use only.

---
