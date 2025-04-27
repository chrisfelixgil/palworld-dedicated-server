# 🎮 Palworld Dedicated Server Docker Setup

[![Docker Pulls](https://img.shields.io/docker/pulls/thijsvanloef/palworld-server-docker?style=for-the-badge)](https://hub.docker.com/r/thijsvanloef/palworld-server-docker)
[![GitHub Stars](https://img.shields.io/github/stars/chrisfelixgil/palworld-dedicated-server?style=for-the-badge)](https://github.com/chrisfelixgil/palworld-dedicated-server)

A powerful and easy-to-deploy Docker setup for running your own Palworld dedicated server. Perfect for hosting your own gaming community or playing with friends!

## ✨ Features

- 🚀 Quick and easy deployment
- 💾 Automatic backups
- 🔄 Auto-restart on crashes
- 🛡️ Secure configuration
- 🎮 Optimized for gaming performance
- 📦 All-in-one Docker solution

## 🏗️ Structure

```
palworld-server/
├── docker-compose.yml    # Server configuration
└── palworld-data/        # Game data and saves
```

## ⚙️ Requirements

- Docker and Docker Compose
- 4GB+ RAM (8GB+ recommended)
- 20GB+ SSD storage
- Open ports: 8211/udp and 27015/udp

## 🚀 Quick Start

1. Clone this repository:
```bash
git clone https://github.com/chrisfelixgil/palworld-dedicated-server.git
cd palworld-dedicated-server
```

2. Configure your server:
   - Edit `docker-compose.yml` and set:
     - `SERVER_PASSWORD`: Server access password
     - `ADMIN_PASSWORD`: Admin password
     - `SERVER_NAME`: Your server name
     - `PLAYERS`: Max number of players

3. Start the server:
```bash
docker-compose up -d
```

4. Check server status:
```bash
docker-compose logs -f
```

## 🔧 Configuration Options

The server comes with optimized settings for:
- 🥚 Egg hatching (2x faster by default)
- 🍖 Food consumption
- ⚔️ PvP settings (friendly fire disabled)
- 🏗️ Building mechanics
- 💀 Death penalties
- And much more!

## 💾 Data Persistence

All game data is stored in the `palworld-data/` directory:
- Game progress
- World saves
- Server configurations
- Automatic backups (4 backups kept)

## 🔒 Security

- Automatic backups every 60 minutes
- Secure password management
- Protected admin access
- Regular updates

## 🤝 Contributing

We love contributions! Here's how you can help:

1. ⭐ Star this repository
2. 🐛 Report bugs
3. 💡 Suggest improvements
4. 📝 Update documentation
5. 🔧 Submit pull requests

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Thanks to all contributors
- Special thanks to the Palworld community
- Inspired by the amazing Docker community

## ⭐ Support Us

If you find this project helpful, please:
- Give it a star ⭐
- Share it with friends
- Consider contributing
- Report any issues

## 📞 Need Help?

- Open an [issue](https://github.com/chrisfelixgil/palworld-dedicated-server/issues)
- Join our Discord community
- Check the FAQ section

Happy gaming! 🎮 