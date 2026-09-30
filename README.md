# homebrew-bridgectl

Homebrew tap for [bridgectl](https://github.com/orchael/bridgectl) — a gRPC daemon and SDK that manages AI agent subprocess lifecycles and exposes a PTY transport.

## Install

```bash
brew install orchael/bridgectl/bridgectl
```

## Notes

- The cask in `Casks/` is generated and committed automatically by GoReleaser during the [Publish CLI](https://github.com/orchael/bridgectl/actions/workflows/publish-cli.yml) workflow. Do not edit it by hand — changes will be overwritten on the next release.
- Released binaries are signed with a Developer ID certificate and notarized by Apple.
- `bridgectl` runs the provider CLIs (`claude`, `codex`, `gemini`, `opencode`) through Node.js 24, which Homebrew does not install for you:

  ```bash
  brew install node@24
  ```

Issues belong on the [main repository](https://github.com/orchael/bridgectl/issues).
