## How does this work

After running devpod up
- The container is created based on .devcontainer/devcontainer.json. In our case it is pointing to a dockerfile.
- The dotfiles repo is cloned to the working directory. In our case: /worspaces/dotfiles.
- The postCreate command is executed from devcointainer.json, which is running two scripts: ./.devcontainer/setup and ./scripts/setup
- .devontainer/setup installs Chezmoi and initializes the dotfiles from this very repository
- script/setup is executed which trusts the dotfiles and the Chezmoi directories.

#### INSTALLATION METHODS
- Chezmoi Externals
  .chezmoiexternals directory
- Mise global c
  dot_config/mise/config.toml
- Mise project (intallation is avaliable only in the directory containing the mise.toml file)

#### SCRIPT RUNNING METHODS
- dotfiles setup
- postCreate (devcontainer.json)
- chezmoiscripts
