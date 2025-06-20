# 🧠 Grid-Based Trading Bot (Hyperliquid + Streamlit)

This project is a fully functional **Grid Trading Bot** built for the **Hyperliquid decentralized exchange**, with a clean and interactive **Streamlit-based interface**. It allows users to create, manage, and run multiple bots using simple UI inputs — no manual scripting required.

---

## 🚀 Features

### ✅ Streamlit Web Interface
- Sidebar navigation for intuitive flow.
- **Dashboard**: View all your bots and control them easily.
- **Create Bot**: Fill a simple form to launch new trading bots.

### ⚙️ Grid Bot Logic (Backend)
- Automatically calculates buy/sell grid levels between user-defined min/max prices.
- Places limit orders on Hyperliquid with proper client order IDs.
- Live monitors fills using `HyperliquidMonitor` and automatically places reverse orders.
- Cancels all open orders before starting a new session for clean execution.

### 🎮 Bot Controls
- Start / Stop bots directly from the UI.
- Edit or Delete any bot with one click.
- Visual feedback for running bots (`Running` button turns green and is disabled).

---

## 🏗️ Project Structure

```bash
.
├── app.py             # Streamlit frontend for bot management
├── bot_logic.py       # Core grid trading logic and Hyperliquid integration
├── dontshareconfig.py # Your private key (not included in repo)
├── requirements.txt   # All necessary Python packages
