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
   sudo mv squashfs-root /
   sudo ln -s /squashfs-root/AppRun /usr/bin/nvim
   ```
2. Install packer
   ```
   git clone --depth 1 https://github.com/wbthomason/packer.nvim\
    ~/.local/share/nvim/site/pack/packer/start/packer.nvim
   ```
3. Clone this repo and start to use
   ```
   git clone https://github.com/wilson-shen/nvim-config.git
   ```
4. Install `build-essential` for linux user, mac/windows I'm not sure do you need this.
   ```
   sudo apt update && sudo apt install build-essential
   ```
5. Go through all lua files in `after/plugin/*.lua` run `:so` once in each file.
6. Again, go through all lua file in `lua/shen/*.lua` and run `:so`, but this time when it comes to `lua/shen/packer.lua`, you will need to run `:PackerSync` after running `:so`.
