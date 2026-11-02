CmdLite

Turn long, complex Minecraft commands into short, easy-to-use shortcuts.

CmdLite is a lightweight Fabric mod that lets you save Minecraft commands in ".txt" files and execute them using simple shortcuts like "/lite:teleport".

Stop typing the same lengthy commands over and over. Save them once, create your shortcuts, and use them whenever you need.

✨ Features

- Custom Command Shortcuts: Execute saved commands using "/lite:<name>".
- Simple File-Based Setup: One ".txt" file creates one command shortcut.
- Multi-Line Support: Store multiple commands in a single file and execute them in order.
- No Artificial Length Limit: CmdLite does not impose its own fixed character limit on saved commands.
- Live Reload: Use "/lite:reload" to load new or updated command files without restarting Minecraft.
- Command List: Use "/lite:list" to view all currently loaded shortcuts.
- No Server-Side Installation Required: Designed to work without requiring the server to install CmdLite.
- Vanilla & Modded Support: Designed for singleplayer and multiplayer environments.

📦 Requirements

- Minecraft
- Fabric Loader
- Fabric API

Make sure you're using versions compatible with your installed Minecraft version and CmdLite release.

📥 Installation

1. Install Fabric Loader for your Minecraft version.
2. Install Fabric API.
3. Download the CmdLite ".jar" file compatible with your Minecraft version.
4. Place the CmdLite ".jar" file inside your Minecraft "mods" folder.
5. Launch Minecraft using your Fabric profile.

🚀 How to Use

1. Create a Command File

Navigate to:

.minecraft/config/cmdlite/commands/

Create a ".txt" file with your desired shortcut name.

Example:

teleport.txt

2. Add Your Command

Open "teleport.txt" and add your Minecraft command:

/tp @s 100 80 100

3. Execute Your Shortcut

Launch Minecraft and run:

/lite:teleport

CmdLite will execute the saved command through Minecraft's normal command system.

That's it! Your shortcut is ready to use.

📝 Multiple Commands

CmdLite supports saving multiple commands in a single file.

Example: "travel.txt"

/tp @s 100 80 100
/time set day
/weather clear

Execute them using:

/lite:travel

Commands are intended to run in order.

Note: Multi-line execution may be affected by command processing, permissions, server behavior, and implementation details.

🔄 Available Commands

Command| Description
"/lite:<name>"| Execute a saved command shortcut
"/lite:reload"| Reload saved command files
"/lite:list"| List currently loaded shortcuts

📂 Folder Structure

.minecraft/
└── config/
    └── cmdlite/
        └── commands/
            ├── teleport.txt
            ├── travel.txt
            └── home.txt

Each ".txt" file represents one shortcut.

For example:

- "teleport.txt" → "/lite:teleport"
- "travel.txt" → "/lite:travel"
- "home.txt" → "/lite:home"

🌐 Compatibility

CmdLite is designed for:

- Minecraft Singleplayer
- Vanilla Multiplayer Servers
- Modded Multiplayer Servers

No server-side CmdLite installation is required by design.

CmdLite sends saved commands through Minecraft's normal command system. It does not grant additional permissions or bypass server restrictions.

Whether a command works depends on the server, your permissions, the command itself, and Minecraft's command handling.

Very long commands may still encounter Minecraft or server-imposed limits.

⚠️ Important Notes

- Use valid Minecraft commands in your files.
- Name your files carefully because filenames determine shortcut names.
- Ensure your commands are supported by your Minecraft version and server.
- Only use commands you are authorized to execute.
- Back up important command files before making changes.

🛠️ Troubleshooting

Shortcut not appearing?

- Check that the file is inside "config/cmdlite/commands/".
- Verify that the file has a ".txt" extension.
- Run "/lite:reload".
- Check for invalid filenames or file contents.

Command not working?

- Verify the command syntax.
- Check your server permissions.
- Test whether the original command works when entered normally.

Changes not showing?

- Run "/lite:reload" and check "/lite:list".

📄 License

Check the repository's license file for the applicable license and usage permissions.

---

CmdLite — Save commands. Create shortcuts. Play smarter.
