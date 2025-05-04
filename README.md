Local Game Manager

Local Game Manager is a cross-platform desktop application built with Tauri and Svelte. It provides a convenient interface to organize and launch your locally installed games.
✨ Features

    🎮 Manage Local Games: Add, edit, and delete games with custom names, icons, and paths

    ⚡ One-Click Launch: Quickly start games directly from the app

    🗂️ Custom Categories: Group your games by genre, platform, or tags

    🔍 Fast Search: Instantly find games with a responsive search bar

    🖼️ Icon Support: Add custom icons for a personalized library

    🔐 Privacy-Friendly: Fully offline – all data is stored locally

🚀 Getting Started
Prerequisites

    Node.js (v18+ recommended)

    Rust

    Tauri CLI

Installation

git clone https://github.com/yourusername/local-game-manager.git
cd local-game-manager
npm install
npm run tauri dev

This will start the development server and launch the Tauri app.
🧩 Technologies Used

    Frontend: Svelte with TypeScript

    Backend / Shell: Tauri powered by Rust

    UI/UX: Tailwind CSS

🛠 Development Scripts

npm run tauri dev       # Start in development mode
npm run tauri build     # Build the app for production

📌 Roadmap

Game import/export

Cloud sync (optional)

Game time tracking

    Steam/Epic integration (if allowed)

❗ Known Issues

    🛑 Game doesn't launch (Windows):
    Ensure the game path is correct and points to a valid .exe. Also check permissions.

    🧱 App freezes when launching some games:
    This can happen if the game blocks the main thread. Use asynchronous process spawning in Rust.

    🔒 Antivirus flags app:
    Unsigned Tauri apps may trigger warnings. Code signing is recommended for public builds.

    🔤 Special characters in paths cause issues:
    Make sure your app properly handles UTF-8 encoded paths, especially on Windows.

❓ FAQ

Q: Does this app require an internet connection?
A: No. All data is stored locally. The app is fully offline-first.

Q: Can I import Steam or Epic games?
A: Not yet. This is planned for a future release.

Q: Where is my game library saved?
A: The library is stored locally via Tauri’s native storage, typically in your OS’s app data directory.

Q: Does this app work on Linux/macOS?
A: Yes. Tauri supports Windows, macOS, and Linux. Just make sure to configure the correct launch paths.

Q: Can I export or back up my library?
A: Exporting is not implemented yet, but you can manually back up the config files.
🤝 Contributing

Contributions are welcome! Please open an issue or pull request if you'd like to help.
📝 License

This project is licensed under the MIT License.