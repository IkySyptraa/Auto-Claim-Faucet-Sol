
# 🚀 Auto-Claim-Faucet SOLANA DEVNET 🤖

A simple, colorful Node.js CLI bot for auto-claiming Solana Devnet faucet airdrop to multiple wallets, with proxy support and countdown timer.

---

## ✨ Features

- **Automatic SOL claim** for all wallets in `wallets.txt`
- **Proxy support** (HTTP/HTTPS/SOCKS5) via `proxies.txt` (or direct if empty)


## 📦 Installation

1. **Clone this repo** (or download the files):

   ```
   git clone <repo-url>
   cd <folder>
   ```

2. **Install dependencies:**
`  npm install axios https-proxy-agent http-proxy-agent socks-proxy-agent chalk@4
`

3. **Prepare your files:**
   - `wallets.txt` — one Solana address per line.
   - `proxies.txt` — one proxy per line, or leave empty for direct connection.

---

## 🚦 Usage

`
node index.js
`

- **interval** (optional) — claim interval in seconds (default: 86400, i.e. 24 hours).
  - Example: `node index.js 60` (claim every 60 seconds)

---

## 📄 File Structure

```
.
├── index.js
├── wallets.txt
├── proxies.txt
└── README.md
```

---

## 📝 Example Output

```
=========================================
🚀 Auto-Claim-Faucet SOLANA DEVNET 🚀 🤖
created by : @PetrukStar
EVM address: 0x2E8cF27819D18D935596915c4066E8198cBEd795
=========================================
⚠️  WARNING: Do not use this script to spam the faucet! Please use it responsibly.

⏳ Auto claim is active every 60 seconds... (Press Ctrl+C to stop)

🌐 Testing proxy: socks5://123.123.123.123:1080 ... 🟢 [OK]
🎉 8UqZp...fke: Claimed 1 SOL successfully! Tx: 123456abcde
🎉 9Jd6a...1gx: Claimed 1 SOL successfully! Tx: 78910fghijk

✅ One round finished. Waiting 60 seconds for the next round...

⏳ Next round in 59 seconds...
⏳ Next round in 58 seconds...
...
```

---

## 🙏 Credits

- Script by **@PetrukStar**
- Inspired by Solana faucet

---

## ⚠️ Disclaimer

- **For educational purposes only.**  
- Do not use to spam faucets or for malicious activity.

