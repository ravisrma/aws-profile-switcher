# 📦 **AWSCTX** — AWS Profile Switcher & Manager

**AWSCTX** is a beautiful, interactive Bash utility for managing multiple AWS profiles. Effortlessly add, remove, rename, copy, and switch between profiles with fuzzy search, color output, and tab completion. 

---

## 🚀 **Features**

- 🔍 **Interactive Profile Switching** — Fuzzy search to switch your default AWS profile
- ➕ **Add Profiles** — Guided prompts for credentials, region, and MFA
- 📋 **List Profiles** — See all profiles, with the current default highlighted
- 🗑️ **Remove Profiles** — Safe deletion with confirmation
- ✏️ **Rename & Copy Profiles** — Rename or duplicate profiles instantly
- 👀 **Show Profile Details** — Display credentials and config for any profile
- ⌨️ **Tab Completion** — Smart completion for commands and profile names
- 🛡️ **Automatic Backup** — Credentials/config files backed up before changes


---

## ⚠️ **Prerequisites**

- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)
- [fzf](https://github.com/junegunn/fzf) (for interactive selection)

Install fzf:
```sh
sudo apt update && sudo apt install fzf -y
```

---

## �️ **Installation**

```sh
# 1. Clone the repo
git clone https://github.com/ravisrma/aws-profile-switcher.git
cd aws-profile-switcher

# 2. Make it executable and install
chmod +x awsctx
sudo mv awsctx /usr/local/bin/
```

That's it! Now you can use `awsctx` from anywhere in your terminal.

---

## ⚡ **Usage**

```bash
awsctx [command] [profile]
```

| Command                | Description                                   |
|------------------------|-----------------------------------------------|
| `awsctx`               | Interactively switch the default AWS profile  |
| `awsctx add`           | Add a new AWS profile                        |
| `awsctx ls`            | List all available AWS profiles               |
| `awsctx rm <profile>`  | Remove a specific AWS profile                 |
| `awsctx rename <old> <new>` | Rename a profile                      |
| `awsctx copy <src> <dest>`  | Copy a profile                        |
| `awsctx show <profile>`| Show profile details                         |
| `awsctx --help`, `-h`  | Show help message                            |

---

## 📝 **Examples**

```bash
awsctx           # Switch profile interactively
awsctx add       # Add a new profile
awsctx rm dev    # Remove the 'dev' profile
awsctx rename dev staging   # Rename 'dev' to 'staging'
awsctx copy prod backup     # Copy 'prod' to 'backup'
awsctx show prod # Show details for 'prod'
```

---

## 💡 **Tips**

- 🛡️ Always back up your AWS credentials before making changes
- ⌨️ Use tab completion for faster command and profile selection
- 🐚 Compatible with Bash and Zsh

---

## 🙏 **Credits**

Created by Ravi Sharma. Contributions welcome!
