# 🐧 eos-commands.sh

An easy to read, colorized 'cheat sheet' that runs in your terminal window to display helpful Linux commands. Originally inspired by using EndeavourOS, but designed for any Arch-based distribution.

---

## 📌 Summary

When executed, this script prints categorized command references directly to your terminal, including:

- 📦 Package Management 
- 📊 System Monitoring
- 🌐 Networking
- 🔒 Firewall & Security
- 📁 File Management
- 👥 Users & Permissions
- ⚙️ Process Control
- 🖥️ Device & App Logging
- 🐙 Git Basics

---

## 📸 Preview

Here's a small snippet of what you'll see when launching your terminal with `eos-commands.sh` enabled:

![commands](https://github.com/user-attachments/assets/a91bb200-8284-402e-b560-0373bc1fe89a)


---

## 🧰 Requirements

- Bash (or compatible shell such as Zsh)
- Terminal with ANSI 256-color support

**Note**:

The majority of commands listed in this script relate to commonly used Linux applications, and as such require prior package installation of the application and/or its dependencies.

For example, if typing a command such as `btop` returns: `command not found` you will need to install it first using a package manager such as pacman, using `sudo pacman -S btop`.

---

## 🛠️ Installation

**Note**:

Make sure to replace `/your/file/path/` with the actual file path on *your* system.
  
1. **Clone the repository**:
   ```bash
   git -c https://github.com/ClayArch/eos-commands.git
   
2. **Make the script executable**:
   ```bash
   chmod +x /your/file/path/eos-commands.sh

3. **(Option 1) Run the script manually**:
   
   ./ means "run the file from the current directory".
   ```bash
   ./eos-commands.sh
   ```
   If you're in a different directory, you'll need to navigate (cd) to where the script is located first.

4. **(Option 2) Run automatically on Terminal Launch**:
   
   Open your shell config file. You can use either the CLI or GUI for this step:
   - For Bash: `~/.bashrc`
   - For Zsh: `~/.zshrc`

   (Beginner-friendly) Add this line at the end of the file:
   
   `bash /your/file/path/eos-commands.sh`
   
   (Advanced-will only run in interactive terminals) Add this line at the end of the file:
   ```
   if [[ $- == *i* ]]; then
     /your/file/path/eos.commands.sh
   fi
   ```

---
