# Username Generator

A Python tool that generates meaningful usernames and checks their availability across popular websites and social media platforms.

## Features

- **Smart Username Generation**: Creates meaningful, short usernames using real words
- **Availability Checking**: Checks if usernames are available on major platforms
- **Advanced Bypass Techniques**: Uses sophisticated methods to check availability even on protected sites
- **Multiple Generation Styles**: Various approaches to create different types of usernames

## Supported Platforms

| Platform | Status | Description |
|----------|--------|-------------|
| GitHub | Working | Code repository hosting |
| Twitter/X | Working | Social media platform |
| Instagram | Working | Photo sharing platform |
| TikTok | Working | Short video platform |
| YouTube | Working | Video sharing platform |
| Snapchat | Working | Photo messaging app |
| Steam | Working | Gaming platform |
| Discord | Manual | Gaming communication platform |
| Reddit | Manual | Discussion platform |
| Twitch | Manual | Live streaming platform |
| Spotify | Manual | Music streaming service |
| LinkedIn | Manual | Professional networking |

## Installation

1. Make sure you have Python 3.7+ installed
2. Install the required dependencies:
```bash
pip install requests
```

## Usage

### Basic Usage

Generate 5 usernames:
```bash
python username_generator.py -g 5
```

### Check Availability

Generate usernames and check availability on GitHub:
```bash
python username_generator.py -g 3 -c github
```

### Generation Styles

**Minimal** (short, meaningful words):
```bash
python username_generator.py -g 3 -s minimal
```

**Word Mash** (combines words):
```bash
python username_generator.py -g 3 -s word_mash
```

**Letter Substitution** (replaces letters with numbers/symbols):
```bash
python username_generator.py -g 3 -s letter_sub
```

**Pronounceable Random** (random but readable):
```bash
python username_generator.py -g 3 -s pronounceable_random
```

### Command Line Options

- `-g, --generate N`: Generate N usernames (default: 5)
- `-s, --style STYLE`: Username generation style
- `-c, --check WEBSITE`: Check availability on specific website
- `--list`: Show supported websites
- `-h, --help`: Show help message

## How It Works

### Username Generation

The tool prioritizes meaningful words over random characters. It uses:
- Real adjectives and nouns
- Letter substitutions (e.g., 'a' → '@', 'e' → '3')
- Word combinations
- Numbers only as a last resort

### Availability Checking

For platforms with anti-bot protection, the tool uses advanced techniques:
- Cookie management and session persistence
- Realistic browser headers and user agents
- Random delays and human-like behavior
- Multiple request patterns to avoid detection
- Content analysis to determine availability

## Examples

```bash
# Generate 3 minimal usernames
python username_generator.py -g 3 -s minimal
# Output: code, data, flow

# Check if 'devuser' is available on GitHub
python username_generator.py -g 1 -c github
# Output: devuser - Available on GitHub

# Generate word mash usernames
python username_generator.py -g 2 -s word_mash
# Output: codeflow, datastream
```

## Technical Details

The tool includes sophisticated bypass techniques for platforms that block automated requests:
- **Header Spoofing**: Mimics real browser requests
- **Session Management**: Maintains cookies and sessions
- **Rate Limiting**: Uses random delays to avoid detection
- **Content Analysis**: Analyzes page content to determine availability
- **Multiple Endpoints**: Tries different API endpoints for each platform

## Requirements

- Python 3.7 or higher
- requests library
- Internet connection for availability checking

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to submit issues, feature requests, or pull requests to improve the tool.