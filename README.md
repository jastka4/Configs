# Config files (aka dotfiles)

## Installation

> :bulb: Install WSL2 when running Windows 10. You can find a guide [here](https://docs.microsoft.com/pl-pl/windows/wsl/install-win10). Also, install the  [Windows Terminal](https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab) that you can download from the Microsoft Store.

### 1. Install Zsh

Use the following [instructions](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH).

### 2. Install Oh My Zsh!

You can access the installation guide [here](https://github.com/ohmyzsh/ohmyzsh/wiki/Installing-ZSH).

```zsh
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

### 3. Install Powerlevel10k

Use the following command:

```zsh
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

Then you need to enable it, change the value of `ZSH_THEME` to following in the `~/.zshrc` file:

```zsh
ZSH_THEME="powerlevel10k/powerlevel10k"
```

## Configuration

### 1. Download FiraCode NF font

You can get the font from [here](https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/FiraCode/Medium/complete/Fira%20Code%20Medium%20Nerd%20Font%20Complete.ttf).

On Windows use [this one](https://github.com/ryanoasis/nerd-fonts/raw/master/patched-fonts/FiraCode/Medium/complete/Fira%20Code%20Medium%20Nerd%20Font%20Complete%20Windows%20Compatible.ttf).

### 2. Configure Powerlevel10k

Type the command below and choose you style options:

```zsh
p10k configure
```

### 3. Install plugins

#### 1. Clone `zsh-syntax-highlighting`

```zsh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

#### 2. Clone `zsh-autosuggestions`

```zsh
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

#### 3. Install `exa`

For an installation guide please head [here](https://the.exa.website/install).

When using Ubuntu version lower than 20.10, use the following commands:

```zsh
wget http://archive.ubuntu.com/ubuntu/pool/universe/r/rust-exa/exa_0.9.0-4_amd64.deb
sudo apt-get install ./exa_0.9.0-4_amd64.deb
```

#### 4. Add plugins to `.zshrc`

```zsh
plugins=( git zsh-syntax-highlighting zsh-autosuggestions )
```

### 4. Copy configs

Copy all configs to your `~/` home directory.
