# hytale-server-downloader (unofficial)

A tiny, **unofficial** Node.js script I hacked together in ~10 minutes to download the latest Hytale server release using the **device code** login flow.

I wrote this because I’m running my server on **ARM64** and the official downloader binary didn’t work, so I needed a simple way to fetch updates for my server files.  
**Don’t expect ongoing support/updates** — I’ll only touch this again if I personally need it.

## What it does
- Starts an OAuth **device login** flow (prints a login link)
- Saves tokens locally to avoid logging in every time
- Checks the latest server release version
- Downloads the `.zip` if a newer version exists

## Requirements
- Node.js 18+ (recommended: Node 20+)

## Usage
```bash
node main.js
