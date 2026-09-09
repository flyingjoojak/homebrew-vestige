# Homebrew tap for Engram

[Engram](https://github.com/flyingjoojak/engram) — your AI coding assistant forgets everything; now you don't have to. Local semantic search over your Claude Code and Codex conversations.

## Install (macOS)

```bash
brew tap flyingjoojak/engram
brew install --cask engram
```

Homebrew removes the quarantine flag for you (the app is unsigned), so there's no Gatekeeper warning, and it keeps the app up to date:

```bash
brew upgrade --cask engram
```

The cask (`Casks/engram.rb`) points at the latest `.dmg` on the [Engram releases page](https://github.com/flyingjoojak/engram/releases).
