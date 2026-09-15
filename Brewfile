# Brewfile for ~/.config/nvim (kickstart.nvim, vim.pack edition)
#
# Install everything with:
#   brew bundle --file ~/.config/nvim/Brewfile
#
# Not in this file (can't be installed via Homebrew):
#   xcode-select --install   -> clang + make (telescope-fzf-native, LuaSnip jsregexp, treesitter parsers)
#
# Language servers, formatters and linters (lua_ls, stylua, marksman, ts_ls,
# eslint, tailwindcss, prettierd, markdownlint, black, isort, ...) are NOT
# listed here: Mason installs them itself from the `servers` table and
# `ensure_installed` list in init.lua.

# --- Editor ---------------------------------------------------------------
brew "neovim"

# --- Search & navigation (telescope.nvim) ---------------------------------
brew "ripgrep"          # <space>sg live grep, <space>sw grep word
brew "fd"               # faster <space>sf find files, respects .gitignore

# --- Syntax (nvim-treesitter, main branch) --------------------------------
brew "tree-sitter"      # CLI required to build/update parsers (:TSUpdate)

# --- Runtimes Mason needs to install tools --------------------------------
brew "node"             # npm: ts_ls, eslint, tailwindcss, cssls, html, jsonls, prettierd, markdownlint
brew "python"           # pip: black, isort

# --- Version control (vim.pack, gitsigns) ---------------------------------
brew "git"              # Apple's bundled git also works; this keeps it current

# --- Terminal & font ------------------------------------------------------
cask "ghostty"                          # the terminal you're using
cask "font-jetbrains-mono-nerd-font"    # required: vim.g.have_nerd_font = true (set as Ghostty font)
