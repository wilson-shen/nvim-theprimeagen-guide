# My Neovim config
Thanks to @ThePrimeagen's guide on "0 to LSP" youtube video.

Most of the keymaps are following his setup, but not theme and Harpoon.

Also some plugins in my config like Harpoon and lsp-zero are using the up-to-date version.

### Steps from download Neovim to use this configure
1. Install Neovim
   ```
   curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim.appimage
   chmod u+x nvim.appimage
   ./nvim.appimage
   ./nvim.appimage --appimage-extract
   ./squashfs-root/AppRun --version
   ```
2. Install packer
   ```
   git clone --depth 1 https://github.com/wbthomason/packer.nvim\ ~/.local/share/nvim/site/pack/packer/start/packer.nvim
   ```
3. Clone this repo and start to use
   ```
   git clone https://github.com/wilson-shen/nvim-config.git
   ```
