# 🎵 Wick Music Bot 🎵

![Wick Music Banner](https://media.wickdev.me/74ayiutgVH.png)

**Wick Music Bot** is a feature-rich Discord bot designed to provide seamless music playback and management within your Discord servers. Powered by the latest technologies and crafted with care by **Wick Studio**, this bot ensures that your community enjoys a top-notch musical experience.

## 🛠️ Features

- **High-Quality Music Playback:** Supports a wide range of platforms including YouTube, SoundCloud, Spotify, and more.
- **Intuitive Commands:** Simple and effective commands for playing, pausing, skipping, and managing the music queue.
- **Interactive Buttons:** Control the music directly from Discord messages with interactive buttons.
- **Customizable Settings:** Tailor the bot's behavior to suit your server's needs with extensive configuration options.
- **Multi-Language Support:** Currently supports Arabic and English, with the ability to add more languages.
- **Robust Error Handling:** Ensures smooth operation with comprehensive error handling and logging.
- **Professional Branding:** Custom music cards and stylish console logs enhance the overall experience.
- **Role-Based Permissions:** Control who can manage the music with DJ role configurations.

## 📦 Installation

### 🔧 Prerequisites

- **Node.js:** Ensure you have [Node.js](https://nodejs.org/) installed (v16.9.0 or higher).
- **Discord Account:** A Discord account to manage your server and bot.
- **Discord Server:** Access to a Discord server where you have permissions to add bots.

### 🚀 Getting Started

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/wickstudio/discord-music-bot.git
   cd discord-music-bot
   ```

2. **Install Dependencies:**

   ```bash
   npm install
   ```

3. **Configure the Bot:**

   - Rename `config.example.js` to `config.js`.
   - Fill in the required fields in `config.js` with your bot's token, client ID, and other configurations.

   ```javascript
   // config.js

   module.exports = {    
       token: "YOUR_BOT_TOKEN", // Your bot's token
       clientId: "YOUR_CLIENT_ID", // Your bot's client ID
       prefix: "!", // Command prefix
       language: "en", // 'ar' for Arabic | 'en' for English
       verbose: true,
       musicCardPath: "./musicard.png",
       enableLogging: true,
       djRoleName: "DJ",
       aliases: {
         play: ["p", "start", "playmusic"],
         pause: ["hold", "stopmusic"],
         resume: ["r", "continue"],
         skip: ["s", "next", "jump"],
         stop: ["end", "terminate"],
         volumeUp: ["vup", "increasevolume"],
         volumeDown: ["vdown", "decreasevolume"],
         repeat: ["loop"],
         queue: ["q"],
         nowplaying: ["np"],
         clear: ["c"],
         remove: ["rm", "delete"]
       }
   };
   ```

4. **Register Custom Fonts:**

   - Ensure you have the Roboto font files (`Roboto-Bold.ttf`, `Roboto-Regular.ttf`, `Roboto-Italic.ttf`) in the `src/fonts` directory.

5. **Run the Bot:**

   ```bash
   npm start
   ```

   If everything is set up correctly, you should see console logs indicating that the bot is online.

## 📝 Configuration

The `config.js` file allows you to customize the bot's behavior. Below are the available configurations:

- **token:** Your Discord bot token.
- **clientId:** Your Discord bot's client ID.
- **prefix:** The prefix used for bot commands (e.g., `!play`).
- **language:** Set to `'ar'` for Arabic or `'en'` for English.
- **verbose:** Enable or disable verbose logging.
- **musicCardPath:** Path to the custom music card image.
- **enableLogging:** Toggle logging of events and errors.
- **djRoleName:** Name of the role that has DJ permissions.
- **aliases:** Define command aliases for easier access.

## 🎮 Usage

Once the bot is running and added to your server, you can use the following commands to control music playback:

### 🎶 Music Commands

| Command          | Aliases                     | Description                             |
| ---------------- | --------------------------- | --------------------------------------- |
| `!play <song>`   | `!p`, `!start`, `!playmusic`| Play a song from YouTube or a supported platform. |
| `!pause`         | `!hold`, `!stopmusic`       | Pause the currently playing song.       |
| `!resume`        | `!r`, `!continue`           | Resume a paused song.                    |
| `!skip`          | `!s`, `!next`, `!jump`      | Skip the currently playing song.         |
| `!stop`          | `!end`, `!terminate`         | Stop the music and clear the queue.       |
| `!volumeUp`      | `!vup`, `!increasevolume`   | Increase the volume by 10%.               |
| `!volumeDown`    | `!vdown`, `!decreasevolume` | Decrease the volume by 10%.               |
| `!repeat`        | `!loop`                      | Toggle the repeat mode.                   |
| `!queue`         | `!q`                         | Display the current music queue.          |
| `!nowplaying`    | `!np`                        | Show the song currently playing.          |
| `!clear`         | `!c`                         | Clear the music queue and stop playback.  |
| `!remove <number>`| `!rm`, `!delete`             | Remove a specific song from the queue.    |

### 📟 Interactive Buttons

The bot also provides interactive buttons directly within Discord messages for quick control:

- **Pause:** ⏸
- **Resume:** ▶️
- **Skip:** ⏭️
- **Stop:** ⏹️
- **Volume Up:** 🔊
- **Volume Down:** 🔉
- **Repeat:** 🔁
- **Open:** 🔗 (Opens the song in a new tab)

## 📚 Localization

Wick Music Bot supports multiple languages. Currently, it supports:

- **English (`en`)**
- **Arabic (`ar`)**

You can set your preferred language in the `config.js` file.

## 🖥️ System Requirements

- **Node.js:** v16.9.0 or higher
- **Discord Account:** To manage and invite the bot
- **Discord Server:** Where you have permissions to add bots

## 🤝 Contributing

Contributions are welcome! If you'd like to contribute to Wick Music Bot, please follow these steps:

1. **Fork the Repository**
2. **Create a Feature Branch**

   ```bash
   git checkout -b feature/YourFeature
   ```

3. **Commit Your Changes**

   ```bash
   git commit -m "Add some feature"
   ```

4. **Push to the Branch**

   ```bash
   git push origin feature/YourFeature
   ```

5. **Open a Pull Request**

Please ensure your contributions adhere to the existing code style and include relevant documentation.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

## 📞 Contact

For support or inquiries, reach out through the following channels:

- **Discord:** [discord.gg/wicks](https://discord.gg/wicks)
- **YouTube:** [@wick_studio](https://youtube.com/@wick_studio)
- **Instagram:** [@mik__subhi](https://instagram.com/mik__subhi)
- **GitHub:** [wickstudio](https://github.com/wickstudio)

---

![Wick Studio](https://media.wickdev.me/IGG6cyadBh.png)