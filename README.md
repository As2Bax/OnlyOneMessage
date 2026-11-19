<img src="https://github.com/user-attachments/assets/5e3734f7-2d67-44a3-9007-d8fc6f07a476" width="250"/>

# OnlyOneMessage

### Command Every Message.

[![Python 3.12+](https://img.shields.io/badge/python-3.12%2B-blue)](https://www.python.org/)
[![License: AGPL-3.0](https://img.shields.io/badge/License-AGPL--3.0-blue.svg)](https://www.gnu.org/licenses/agpl-3.0.html)
[![Discord.py](https://img.shields.io/badge/discord.py-latest-blue)](https://github.com/Rapptz/discord.py)


## ❓ Overview

OnlyOneMessage is a feature-rich Discord bot that provides server admins **complete control** over text channel behavior.
Set slowmodes **surpassing Discord's limit**, log **individual member cooldowns**, and **fine-tune** settings for **each individual channel**;
all through a straightfoward interface using Discord's slash commands.

📎 Visit the website: [onlyonemessage.as2bax.dev](https://onlyonemessage.as2bax.dev)

❓ Documentation: [onlyonemessage.as2bax.dev/docs](https://onlyonemessage.as2bax.dev/docs)


## ⚡ Features

- **⏳ Advanced Slowmode Control** - Set channel slowmodes lasting hours, days, **or even indefinitely**; surpassing Discord's limitations.
- **💬 Smart Message Management** - Allow members to **chat again** once they delete their message, providing complete flexibility in message flow.
- **📝 Detailed Logging** - Automatically log when members enter slowmode **and when they expire**, including other essential options
- **📊 Analytics** - Built-in Prometheus tracking for reliability 
- **🐬 Docker Supported** - Containerized deployment with Docker for easy usage


## 🖥️ Installation

OnlyOneMessage is fully supported **and** hosted for free, [invite the bot here.](https://onlyonemessage.as2bax.dev/invite)
If you would like to self-host this bot, follow the instructions below:

### Prerequisites

- Python (**3.10+** recommended)
- Docker
- Discord bot token (Get one from the Discord Developer Portal)

> [!NOTE]
> OnlyOneMessage uses `MongoDB` for its database; a self-hosted setup has already been provided in `docker-compose.yml`. Edit if needed.

### Instructions

1. Clone the repository:
```bash
git clone https://github.com/As2Bax/OnlyOneMessage.git
cd OnlyOneMessage
```

If you'd like to use the nightly branch:
```bash
git clone -b nightly https://github.com/As2Bax/OnlyOneMessage.git
cd OnlyOneMessage
```

> [!WARNING]
> The `nightly` branch of OnlyOneMessage is a **beta build of a later version**, expect bugs when using it.

2. Configure the bot

Duplicate the file `.env.example` inside `data`. Name it `.env`, and fill in what's requested.


4. Run the bot:
```bash
docker compose up -d
```

The bot will automatically install dependencies and start the container with automatic restart enabled. To view the container's logs:
```bash
docker logs -f onlyonemessage
```

### Uninstallation

Simply run this in the root directory:
```bash
docker compose down -v
```

> [!WARNING]
> `-v` will clear all volumes related to OnlyOneMessage, **including it's database.** If you wish to keep it's database, leave `-v` out.


## 🛠️ Contributing to OnlyOneMessage

We welcome contributions to OnlyOneMessage from the community! 
Your help is appreciated, whether you're adding features, fixing bugs, or adding documentation.

> [!NOTE]
> If you are going to make major changes to OnlyOneMessage, **open an issue first** to discuss before investing time in it.

### Contributions We Welcome

- **Bug Fixes** - Issues and their solutions
- **Features** - Command improvements/new functions
- **Documentation** - README improvements, code comments, documentation under [OnlyOneMessageWeb](https://github.com/As2Bax/OnlyOneMessageWeb)
- **Refactoring** - Quality of life changes, code quality improvements

### Getting Started

1. Fork this repository

2. Clone your fork:
```bash
git clone https://github.com/<YOUR_USERNAME>/OnlyOneMessage.git
cd OnlyOneMessage
```

3. Create a branch on your fork:
```bash
git checkout -b <BRANCH>/<YOUR_CHANGE>
```

4. Continue setting up the bot through the `Installation` section

### Making Changes

Here's a checklist on what your changes should follow:

- Keep commits clean; each commit should be logical
- Follow the existing style with the codebase unless necessary to change it
- Add comments for logic that isnt obvious

### Before making a Pull Request

- Verify your changes work in a **testing server**
- Submit **one** change per pull request (exceptions apply)
- Update documentation if your changes affect this README or comments

### Submitting your Changes

1. Push to your fork, if you haven't

2. Open a **Pull Request** on this repository with the following:
    - A clear title describing your changes
    - A detailed description on what you've done
    - Reference related issues if needed
    - Screenshots/logs if necessary

4. Respond and edit to changes if requested

### Questions?

If you have any questions regarding this, see our `Support` section, open a new issue, or check our documentation for further details.

Thank you for contributing! 💖


## 📰 License

This project is licensed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**, see the `LICENSE.txt` file for more information.


## ❓ Support
You can receive support by [joining our support server](https://onlyonemessage.as2bax.dev/support), creating an issue on this repository, or by [emailing us.](mailto:support@as2bax.dev)

---

**Made with ❤️ by [As2Bax](https://as2bax.dev)**