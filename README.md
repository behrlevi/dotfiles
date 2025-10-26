## How does this work

- Devpod up . clones the dotfiles repo to /worspaces/dowfiles.
- The contents of .devctontainer/devcontainer.json is read which contains a post create command.
- The .devontainer/setup installs Chezmoi.
- The script/setup is executed which trust the dotfiles and the Chezmoi directories.
- 
