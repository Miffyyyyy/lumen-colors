# Lumen - Discord Color Role Bot

## 🚀 Bot Invite Link

```bash
   https://discord.com/oauth2/authorize?client_id=1392550741217906789&permissions=268528880&integration_type=0&scope=bot+applications.commands 
   ```
A professional Discord bot that provides a beautiful color role system with aesthetic color shades and reaction-based role assignment.

## ✨ Features

- **🎨 8 Color Families**: Red, Pink, Orange, Yellow, Green, Blue, Purple, Brown
- **🌈 12+ Shades per Family**: Each color family has 12+ beautiful aesthetic shades
- **⚡ Easy Setup**: Simple `/setup` command to configure the system
- **🔄 One Role Per User**: Users can only have one color role at a time
- **💾 Persistent Storage**: Server configurations are saved and persist through bot restarts
- **🛡️ Professional**: Comprehensive error handling and permission checks
- **🎯 Modular Design**: Clean, organized code structure


### Bot Setup

1. **Invite the bot to your server** with these permissions:
   - Manage Roles
   - Send Messages
   - Use Slash Commands
   - Read Message History
   - Add Reactions

2. **Run the setup command:**
   ```
   /setup #channel
   ```

3. **Enjoy!** Users can now react to get their color roles.

## 📋 Commands

| Command | Description | Permission Required |
|---------|-------------|-------------------|
| `/setup #channel` | Setup color role system in specified channel | Manage Server |
| `/delete` | Remove color role system from server | Manage Server |

## 🎨 Color Families

### Red Family (🍒)
- Cherry Red, Crimson, Ruby, Scarlet, Burgundy, Rose Red, Coral Red, Maroon, Pink Red, Blood Red, Sunset Red, Pastel Red

### Pink Family (🎀)
- Pastel Pink, Hot Pink, Deep Pink, Light Pink, Rose Pink, Magenta, Fuchsia, Salmon Pink, Peach Pink, Cotton Candy, Blush, Bubblegum

### Orange Family (🍊)
- Sunset Orange, Tangerine, Coral, Peach, Amber, Burnt Orange, Pumpkin, Apricot, Salmon, Golden Orange, Terracotta, Mango

### Yellow Family (⭐)
- Golden Yellow, Lemon, Canary, Sunshine, Cream, Honey, Butter, Daffodil, Banana, Corn, Marigold, Pastel Yellow

### Green Family (🌿)
- Emerald, Forest Green, Lime, Sage, Mint, Olive, Jade, Sea Green, Grass, Pine, Kelly Green, Pastel Green

### Blue Family (💙)
- Ocean Blue, Sky Blue, Navy, Royal Blue, Turquoise, Cobalt, Azure, Sapphire, Teal, Cornflower, Steel Blue, Pastel Blue

### Purple Family (💜)
- Royal Purple, Lavender, Violet, Plum, Orchid, Amethyst, Indigo, Mauve, Magenta, Grape, Lilac, Pastel Purple

### Brown Family (🍫)
- Chocolate, Caramel, Coffee, Tan, Beige, Chestnut, Mocha, Sienna, Khaki, Walnut, Cocoa, Pastel Brown

## 🔧 Configuration

### Bot Permissions
The bot requires these permissions:
- **Manage Roles**: To create and manage color roles
- **Send Messages**: To post color role messages
- **Use Slash Commands**: To respond to commands
- **Read Message History**: To manage reactions
- **Add Reactions**: To add reaction options

### Role Settings
- All color roles have **no permissions** (clean slate)
- Roles are **not hoisted** (don't appear separately)
- Roles are **not mentionable**
- Users can only have **one color role at a time**

## 📁 File Structure

```
lumen-bot/
├── commands/
│   ├── setup.js          # Setup command
│   └── delete.js         # Delete command
├── handlers/
│   └── reactionHandler.js # Reaction event handlers
├── utils/
│   └── colorManager.js   # Color role management utilities
├── config.json           # Bot configuration and color definitions
├── index.js              # Main bot file
├── deploy-commands.js    # Command deployment script
├── package.json          # Dependencies
└── README.md            # This file
```

## 🛠️ Development

### Adding New Colors
To add new color families or shades, edit the `colorFamilies` object in `config.json`:

```json
{
  "newColor": {
    "name": "New Color",
    "emoji": "🎨",
    "shades": [
      {
        "name": "Shade Name",
        "hex": "#HEXCODE",
        "emoji": "🎨"
      }
    ]
  }
}
```


## 🔒 Security Features

- **Permission Checks**: All commands verify bot permissions
- **Error Handling**: Comprehensive error handling throughout
- **Rate Limiting**: Built-in delays to avoid Discord rate limits
- **Input Validation**: All user inputs are validated
- **Safe Role Management**: Roles are created with minimal permissions

## 📊 Server Configuration Storage

Server configurations are stored in `serverConfigs.json` and include:
- Guild ID
- Channel ID for color messages
- Role IDs and metadata
- Message IDs and metadata
- Setup information (who, when)

## 🤝 Support

If you encounter any issues:
1. Check the console for error messages
2. Verify bot permissions
3. Ensure Node.js version is 16.0.0+
4. Check that all dependencies are installed

## 📝 License

This project is licensed under the MIT License.

---

**Made with ❤️ for the Discord community** 
