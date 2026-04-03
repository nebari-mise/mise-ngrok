# mise-ngrok

[mise](https://mise.jdx.dev) plugin for [ngrok](https://ngrok.com).

ngrok distributes binaries through its own CDN with opaque per-version download
tokens, so this plugin maintains a manual mapping of version → token sourced from
[Homebrew's cask](https://github.com/Homebrew/homebrew-cask/blob/main/Casks/n/ngrok.rb).

## Bumping versions

1. Check the [Homebrew cask](https://github.com/Homebrew/homebrew-cask/blob/main/Casks/n/ngrok.rb) for the new version + hashes
2. Add the new entry to the `hashes` array in `bin/install`
3. Update the version in `bin/list-all`
