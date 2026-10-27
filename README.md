# EconomyBank

**EconomyBank** is a lightweight, high-performance banking plugin designed for modern Paper Minecraft servers (1.21+ / 26.x API). It integrates seamlessly with Vault and EconomyShopGUI, giving players a clean GUI menu to deposit and withdraw money, earn periodic interest, and pay custom transaction taxes.

---

## 🌟 Features

* **Interactive GUI Menu**: Open your account with `/bank` or `/b` to make quick deposits and withdrawals ($100 or All balance).
* **Automated Interest**: Periodically rewards players with compound interest on their bank deposits.
* **Custom Tax System**: Automatically deducts configurable tax percentages on deposits and withdrawals to balance the server economy.
* **Vault & EconomyShopGUI Integration**: Hooks into Vault for universal economy support alongside EconomyShopGUI shop transactions.
* **Auto-Generating Config**: Generates `config.yml` on first startup and tracks player bank accounts in `bankdata.yml`.

---

## 🛠️ Installation

1. Download `economybank.jar`[cite: 1].
2. Drop `economybank.jar` into your server's `plugins/` folder.
3. Ensure **Vault** and a compatible economy plugin (e.g., EssentialsX) are installed.
4. Restart your server to generate the default configuration files.

---

## 📋 Commands & Permissions

| Command | Description | Permission | Default |
| :--- | :--- | :--- | :--- |
| `/bank` | Opens the interactive Bank GUI | `economybank.use` | Everyone |
| `/b` | Alias for `/bank` | `economybank.use` | Everyone |

---

## ⚙️ Configuration (`config.yml`)

```yaml
# EconomyBank Configuration File

# Tax rate applied on deposits and withdrawals (0.05 = 5%)
tax-rate: 0.05

# Interest rate applied to player bank balances (0.02 = 2%)
interest-rate: 0.02

# Interval for distributing interest in seconds (3600 = 1 hour)
interest-interval-seconds: 3600
