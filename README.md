# 🎯 Universal Username Generator

A powerful Python tool that generates available usernames for popular websites and apps. Check availability across multiple platforms and find the perfect username for your online presence!

## ✨ Features

- **Multi-Platform Support**: Generate usernames for 12+ popular websites and apps
- **Availability Checking**: Automatically check if usernames are available
- **Multiple Styles**: Random, themed, and minimal username generation
- **Smart Search**: Find available usernames across multiple platforms
- **Interactive Mode**: User-friendly command-line interface
- **Rate Limiting**: Respectful API usage with built-in delays
- **Comprehensive Coverage**: GitHub, Twitter, Instagram, TikTok, Discord, Reddit, YouTube, Twitch, Steam, and more!

## 🚀 Quick Start

### Installation

1. **Clone or download** this repository
2. **Install dependencies**:
   ```bash
   pip install requests
   ```
3. **Run the application**:
   ```bash
   python username_generator.py
   ```

### Interactive Mode (Recommended)

```bash
python username_generator.py
```

Follow the menu to generate and check usernames!

## 🛠️ Usage Examples

### Generate Random Usernames

```bash
# Generate 5 random usernames
python username_generator.py -g 5

# Generate 10 usernames with custom length
python username_generator.py -g 10 -l 12
```

### Generate Themed Usernames

```bash
# Adjective + Noun style (e.g., "coolcode", "epicdev")
python username_generator.py -s adjective_noun -g 5

# Noun + Number style (e.g., "developer", "coder1")
python username_generator.py -s noun_number -g 5

# Minimal style (e.g., "dev", "pro", "ace")
python username_generator.py -s minimal -g 5

# Word Mash style (e.g., "codeart", "techfun")
python username_generator.py -s word_mash -g 5

# Letter Substitution style (e.g., "c0de", "h4ck")
python username_generator.py -s letter_sub -g 5
```

### Check Username Availability

```bash
# Check if "myusername" is available across platforms
python username_generator.py -c myusername
```

### Find Available Username

```bash
# Find an available username automatically
python username_generator.py -f

# Find available username with specific style
python username_generator.py -f -s minimal
```

### Show Supported Platforms

```bash
# List all supported websites and apps
python username_generator.py --list
```

## 🌐 Supported Platforms

| Platform | Auto-Check | Description |
|----------|------------|-------------|
| **GitHub** | ✅ | Code repository hosting |
| **Twitter/X** | ✅ | Social media platform |
| **Instagram** | ✅ | Photo sharing platform |
| **TikTok** | ✅ | Short video platform |
| **Reddit** | ✅ | Discussion platform |
| **YouTube** | ✅ | Video sharing platform |
| **Twitch** | ✅ | Live streaming platform |
| **Steam** | ✅ | Gaming platform |
| **Discord** | ❓ | Gaming communication |
| **Spotify** | ❓ | Music streaming |
| **LinkedIn** | ❓ | Professional networking |
| **Snapchat** | ❓ | Photo messaging |

## 🎨 Username Styles

### 1. Random Style
- **Example**: `bamoki`, `zepula`, `vixuna`
- **Best for**: Unique, pronounceable usernames
- **Features**: Alternating consonants and vowels for readability

### 2. Adjective + Noun Style
- **Example**: `coolcode`, `epicdev`, `zenhack`
- **Best for**: Memorable, branded usernames
- **Features**: Combines descriptive words with tech terms (numbers only as last resort)

### 3. Noun + Number Style
- **Example**: `developer`, `coder1`, `hack2`
- **Best for**: Professional, clean usernames
- **Features**: Uses numbers only when words are too short

### 4. Minimal Style
- **Example**: `dev`, `pro`, `ace`, `code`, `hack`
- **Best for**: Short, clean usernames
- **Features**: 2-6 characters, very meaningful words

### 5. Word Mash Style
- **Example**: `codeart`, `techfun`, `webjoy`
- **Best for**: Creative, memorable combinations
- **Features**: Combines two meaningful words

### 6. Letter Substitution Style
- **Example**: `c0de`, `h4ck`, `t3ch`
- **Best for**: Tech-savvy, leet speak style
- **Features**: Uses numbers that look like letters

## 🔧 Command-Line Options

| Option | Description | Example |
|--------|-------------|---------|
| `-g, --generate COUNT` | Generate usernames | `-g 5` |
| `-s, --style STYLE` | Username style | `-s adjective_noun` |
| `-c, --check USERNAME` | Check availability | `-c myusername` |
| `-f, --find` | Find available username | `-f` |
| `--list` | Show supported platforms | `--list` |
| `-l, --length LENGTH` | Username length | `-l 12` |

## 🎯 Use Cases

### Personal Branding
- **Consistent Username**: Use the same username across all platforms
- **Professional Presence**: Find clean, professional usernames
- **Brand Building**: Create memorable usernames for your brand

### Content Creation
- **Streaming**: Find available usernames for Twitch, YouTube
- **Social Media**: Secure usernames across Instagram, TikTok, Twitter
- **Gaming**: Check availability on Steam, Discord

### Development
- **GitHub**: Secure your developer username
- **Portfolio**: Consistent branding across platforms
- **Open Source**: Professional username for contributions

## 🔒 Privacy & Ethics

- **Rate Limiting**: Built-in delays to respect website resources
- **No Data Storage**: No usernames or personal data are stored
- **Respectful Usage**: Only checks public availability, no account creation
- **Educational Purpose**: Tool for learning about web APIs and availability checking

## 📁 Project Structure

```
username-generator/
├── username_generator.py    # Main application file
├── requirements.txt         # Python dependencies
└── README.md               # This documentation
```

## 🚀 Advanced Features

### Availability Checking Logic
- **404 Status**: Username is available
- **200 Status**: Username is taken
- **Other Status**: Unknown availability
- **Error Handling**: Graceful handling of network issues

### Smart Generation
- **Avoid Conflicts**: Generates unique combinations
- **Length Optimization**: Balances memorability with availability
- **Style Consistency**: Maintains chosen style across generations

### Interactive Features
- **Real-time Feedback**: Shows checking progress
- **Multiple Attempts**: Tries multiple usernames automatically
- **Platform Coverage**: Checks key platforms first

## 🐛 Troubleshooting

### Common Issues

1. **"requests module not found"**
   ```bash
   pip install requests
   ```

2. **"Username checking failed"**
   - Check your internet connection
   - Some platforms may block automated requests
   - Try again after a few minutes

3. **"No available usernames found"**
   - Try a different style
   - Increase max attempts
   - Use longer usernames

### Rate Limiting
- The tool includes built-in delays between requests
- If you get blocked, wait a few minutes before trying again
- Consider using manual checking for sensitive platforms

## 🔮 Future Enhancements

- [ ] More platform support (Facebook, Pinterest, etc.)
- [ ] Username suggestions based on your name
- [ ] Bulk availability checking
- [ ] Username history tracking
- [ ] Web interface version
- [ ] API integration for more platforms
- [ ] Username strength analysis
- [ ] Custom word lists

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature-name`
3. Add new platforms or improve existing features
4. Commit changes: `git commit -m 'Add feature'`
5. Push to branch: `git push origin feature-name`
6. Submit a pull request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- All the platforms for providing public APIs
- The Python community for excellent libraries
- Open source contributors for inspiration

## 💡 Tips for Best Results

- **Start with key platforms**: GitHub, Twitter, Instagram
- **Use consistent styles**: Pick one style and stick with it
- **Check multiple options**: Generate several usernames to choose from
- **Be patient**: Availability checking takes time
- **Keep it simple**: Shorter usernames are often more available

---

**Find your perfect username across the web! 🌐**
