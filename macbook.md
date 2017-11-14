## git
- `brew install git`
- `git config --global pull.rebase true`

## nvm
- `curl -o- https://raw.githubusercontent.com/creationix/nvm/v{LATEST_VERSION}/install.sh | bash`

## Virtual Studio Code
```json
{
    "workbench.iconTheme": "vscode-icons",
    "vim.disableAnnoyingNeovimMessage": true,
    "terminal.integrated.shell.osx": "/bin/zsh",
    "terminal.integrated.fontFamily": "Source Code Pro for Powerline",
    
    "editor.renderWhitespace": "all",
    "files.autoSave": "onFocusChange",
    "editor.wordWrap": "on",
    "vim.insertModeKeyBindings": [
        {
            "before": ["j", "j"],
            "after": ["<esc>"]
        }
   ]
}
```

## zsh & bash

### Installation
- `sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

### .bash_profile

```sh
source ~/.zshrc
```

### .zshrc

```sh
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

alias gp=gulp

ssh-add -K ~/.ssh/id_rsa # to store ssh-key to keychain permanantly with passphrase
```
