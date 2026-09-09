# Homebrew tap for Engram

[Engram](https://github.com/flyingjoojak/engram) — your AI coding assistant forgets everything; now you don't have to. Local semantic search over your Claude Code and Codex conversations.

## Install (macOS, Apple Silicon)

```bash
brew tap flyingjoojak/engram
brew install --cask engram
```

If you see an "untrusted tap" warning, run `brew trust flyingjoojak/engram` and install again.

**After installing**, v0.1.0 isn't code-signed yet, so run this once to make the app open (Apple Silicon blocks unsigned apps as "damaged"):

```bash
xattr -cr /Applications/Engram.app
codesign --force --deep --sign - /Applications/Engram.app
```

This just adds a local ad-hoc signature. A later version will ship signed and drop this step.

Update with `brew upgrade --cask engram`. The cask (`Casks/engram.rb`) points at the latest `.dmg` on the [Engram releases page](https://github.com/flyingjoojak/engram/releases).
