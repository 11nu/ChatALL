<div align="center">
  <img src="src/assets/logo-cover.png" width=256></img>
  <p><strong>Chat with ALL AI Bots Concurrently, Discover the Best</strong></p>

</div>

## Screenshots

![Screenshot](screenshots/screenshot-2.png?raw=true)
![Screenshot](screenshots/screenshot-1.png?raw=true)

## Features

Large Language Models (LLMs) based AI bots are amazing. However, their behavior can be random and different bots excel at different tasks. If you want the best experience, don't try them one by one. ChatALL (Chinese name: 齐叨) can send prompt to several AI bots concurrently, help you to discover the best results.

### Supported bots

| AI Bots                                                                   | Web Access  | API         |
| ------------------------------------------------------------------------- | ----------- | ----------- |
| [ChatGPT](https://chat.openai.com)                                        | Yes         | Yes         |
| [Bing Chat](https://www.bing.com/new)                                     | Yes         | No API      |
| [Bard](https://bard.google.com/)                                          | Yes         | No API      |

And more...

### Other features

- Quick-prompt mode: send the next prompt without waiting for the previous request to complete
- Store chat history locally, protect your privacy
- Highlight the response you like, delete the bad
- Automatically keep ChatGPT session alive
- Enable/disable any bots at any time
- Switch between one, two, or three-column view
- [TODO] Best recommendations

## Prerequisites

ChatALL is a client, not a proxy. Therefore, you must:

1. Have working accounts and/or API tokens for the bots.
2. Have reliable network connections to the bots.
3. If you are using a VPN, it must be set as system/global proxy.

## Download / Install

Download from https://github.com/11nu/ChatALL/releases

### On Windows

Just download the \*-win.exe file and proceed with the setup.

### On macOS

For Apple Silicon Mac (M1, M2 CPU), download the \*-mac-arm64.dmg file.

For other Macs, download \*-mac-x64.dmg file.

### On Linux

Download the .AppImage file, make it executable, and enjoy the click-to-run experience.

## For developers

### Run

```bash
npm install
npm run electron:serve
```

### Build

Node.js must be v16.x

Build for your current platform:

```bash
npm run electron:build
```

If you get the following error using macOS, follow these steps to install Python 2 and build again.

```bash
Error: Exit code: ENOENT. spawn /usr/bin/python ENOENT
```

```bash
pyenv install 2.7.18
PYTHON_PATH=$HOME/.pyenv/versions/2.7.18/bin/python2.7 npm run electron:build
```

Build for all platforms:

```bash
npm run electron:build -- -wml --x64 --arm64
```
