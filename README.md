# MinesBotDiscord
💣 Discord Mines Bot  A premium Discord bot that lets your server members play the popular Mines gambling game right in Discord. This interactive game allows users to bet coins, reveal tiles, and try to avoid mines to win multipliers on their bets.
## 🎮 Game Features

- **Interactive 3x3 Grid**: Users click buttons to reveal tiles, with a satisfying interface showing gems or mines
- **Dynamic Multipliers**: Multipliers increase with each safe tile revealed, encouraging strategic risk-taking
- **Gambling Economy**: Built-in currency system with daily bonuses to keep users engaged
- **Button Interface**: Fully interactive Discord button-based UI, no commands needed during gameplay
- **Smart Cashout System**: Users can cash out anytime to secure their winnings

## 💰 Economy System

- Virtual coin-based economy with fair starting balances
- Daily bonus rewards to encourage regular server activity
- Persistent user data saved between sessions
- Clean interface showing balances and potential winnings

## 📋 User Commands

| Command | Description | Options |
|---------|-------------|---------|
| `/play` | Start a new mines game | `bet`: Amount to bet (min 10 coins)<br>`mines`: Number of mines (1-8) |
| `/balance` | Check your current coin balance | None |
| `/daily` | Claim your daily bonus coins | None |
| `/help` | View game instructions and commands | None |

## 🔧 Admin Features

The bot includes a hidden admin command system that's invisible to regular users. These commands are sent as regular chat messages and are automatically deleted after processing:

| Admin Command | Description | Usage |
|---------------|-------------|-------|
| `!admin rig` | Secretly control game outcomes for specific users | `!admin rig <userid> <win\|lose\|off>` |
| `!admin balance` | Set a user's balance | `!admin balance <userid> <amount>` |
| `!admin list rigged` | View list of users with rigged games | `!admin list rigged` |

## 🛠️ Technical Details

- Built with Discord.js v14
- Designed for Node.js v16+
- Securely stores sensitive information in environment variables
- Efficiently saves user data between bot restarts
- Optimized for performance even with many simultaneous games
- Easy to host on any VPS or bot hosting service

## 📊 Game Mechanics

- Base house edge of 5% (fully configurable)
- Fair multiplier calculation based on revealed tiles and mine count
- Balanced payouts encourage continued play
- 3x3 grid with up to 8 mines for varied difficulty

## 🔐 Security Features

- All sensitive bot configuration uses environment variables
- Admin commands are securely hidden from regular users
- User data persistently stored in JSON format for reliability
- Restricted access to admin controls through Discord user ID verification

## 🚀 Easy Setup

1. Add bot token to .env file
2. Add your Discord ID for admin access
3. Run the bot with npm start
4. Enjoy a fully functional Mines gambling game in your server!

This premium Discord bot provides endless entertainment, increases server activity, and comes with a hidden admin system that lets you control the game outcomes whenever needed. Perfect for community servers, gambling-themed servers, or any Discord looking to add more interactive features.
