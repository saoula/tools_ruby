Tools Ruby
======

A Docker image with a Ruby and a set of ruby tools for web development purposes.

## What's in the image?
- Ruby 2.4.X

### Gems
- bundler
- rubocop
- bundler-audit
- rubycritic

## Usage
To open a shell with all the tools, mounting the current folder:

```docker run --rm -it -v "$(pwd):/app" saoula/tools_ruby sh```

## Alias
### Bash
- Append ```alias rb='docker run --rm -it -v "$(pwd):/app" saoula/tools_ruby'``` to _~/.bashrc_
- Enter `source ~/.bashrc` or open a new terminal window
- Type `rb <command>`, for example `rb irb`
### Zsh
- Append ```alias rb='docker run --rm -it -v "$(pwd):/app" saoula/tools_ruby'``` to _~/.zshrc_
- Enter `source ~/.zshrc` or open a new terminal window
- Type `rb <command>`, for example `rb irb`