# NVIM Config Files

Hier ist ein vollständiges Backup des kompletten NVIM Config Trees.
Ich versuche ihn möglichst aktuell zu halten.

## Installation
Folge den Anweisungen aus dem Repository [.config](https://github.com/favo2244/.config).
Wichtig ist hierbei (Stand 06/2024) nicht die neuste Neovim Version zu nutzen, sondern die version `0.9.x`.

Dazu sind folgende Schritte (in Arch Linux) nötig:
- `sudo pacman -S base-devel cmake unzip ninja tree-sitter curl`
- Nun muss der alte Branch aus dem Nvim Repo kopiert werden, z.B. `release-0.9`
  
  `git clone -b release-0.9 https://github.com/neovim/neovim.git`
- `cd neovim`
- `make CMAKE_BUILD_TYPE=RelWithDebInfo`
- `sudo make install`

Anschließend sollte Neovim installiert sein und kann über `nvim` aufgerufen werden.

Weitere Packages die für NeoVim in dieser Konfiguration installiert sein sollten:
```
sudo pacman -S zathura
sudo pacman -S npm
sudo npm install -g neovim
sudo pacman -S ripgrep
sudo pacman -S latexmk
sudo pacman -S fd
sudo pacman -S biber
sudo pacman -S ruby
gem install neovim
sudo pacman -S wget
sudo pacman -S go
sudo pacman -S php
sudo pacman -S jdk-openjdk
sudo pacman -S julia
sudo pacman -S cargo
sudo pacman -S composer
sudo pacman -S luarocks
sudo pacman -S perl
```
Für zathura muss die entsprechende `zathurarc` in `~/.config/zathura` 


## .config Files

Vorrausgesetzt, das [geforkte Repository](https://github.com/favo2244/.config) ist synchron mit dem [Upstream](https://github.com/benbrastmckie/.config) kann der Pull durchgeführt werden:

```
cd ~/.config
git init
git remote add origin git@github.com:favo2244/.config.git
git pull origin master
```
bzw. für die eigenen Dotfiles:
```
git remote add origin git@github.com:favo2244/NVIM_Config.git
```
Ist der Upstream dem geforkten Repository vorraus, muss dieses zuerst synchronisiert werden.
