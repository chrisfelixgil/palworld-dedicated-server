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
- ⚡ Instant egg hatching
- 🔄 Cross-platform support

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
     - `EGG_HATCHING_SPEED_RATE`: Egg hatching speed (default: 999999.0)
     - `EGG_HATCHING_REQUIRED_TIME`: Required time for hatching (default: 0.000001)
     - `PAL_EGG_DEFAULT_HATCHING_TIME`: Default hatching time (default: 0.000001)

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
- 🥚 Instant egg hatching (configured for immediate hatching)
- 🍖 Food consumption
- ⚔️ PvP settings (friendly fire disabled)
- 🏗️ Building mechanics
- 💀 Death penalties
- And much more!

### Advanced Configuration

You can customize various game settings in the `docker-compose.yml` file:

```yaml
# Game configurations
- DIFFICULTY=Normal
- DAY_TIME_SPEED_RATE=1.0
- NIGHT_TIME_SPEED_RATE=1.0
- EXP_RATE=1.0
- PAL_CAPTURE_RATE=1.0
- PAL_SPAWN_NUM_RATE=1.0

# Incubation configurations
- EGG_HATCHING_SPEED_RATE=999999.0
- EGG_HATCHING_REQUIRED_TIME=0.000001
- PAL_EGG_DEFAULT_HATCHING_TIME=0.000001
```

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
- RCON enabled for remote administration

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