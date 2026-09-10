# Homebrew tap for Vestige

[Vestige](https://github.com/flyingjoojak/vestige) — your AI coding assistant forgets everything; now you don't have to. Local semantic search over your Claude Code and Codex conversations.

## Install (macOS, Apple Silicon)

```bash
brew tap flyingjoojak/vestige
brew install --cask vestige
```

If you see an "untrusted tap" warning, run `brew trust flyingjoojak/vestige` and install again.

**After installing**, v0.1.0 isn't code-signed yet, so run this once to make the app open (Apple Silicon blocks unsigned apps as "damaged"):

```bash
xattr -cr /Applications/Vestige.app
codesign --force --deep --sign - /Applications/Vestige.app
```

This just adds a local ad-hoc signature. A later version will ship signed and drop this step.

Update with `brew upgrade --cask vestige`. The cask (`Casks/vestige.rb`) points at the latest `.dmg` on the [Vestige releases page](https://github.com/flyingjoojak/vestige/releases).
