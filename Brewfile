# Brewfile

###############################################################################
# Xcode Command-Line Tools (not managed by Homebrew)
# Install via `xcode-select --install` to get Apple’s compilers (clang), make,
# git, and system headers required for building native code and Homebrew formulas.
###############################################################################

# Mac App Store CLI to automate App Store installs
brew "mas"

# Install full Xcode (optional GUI IDE + SDKs), which also bundles
# the Command-Line Tools. You can skip if you only need the CLI.
mas "Xcode", id: 497799835
# Xcode: Apple's IDE for iOS/macOS development. Provides Interface Builder,
# Simulator, advanced debugging, and the same compilers/SDKs as `xcode-select`.

mas "Slack-for-Desktop", id: 803453959
mas "whatsapp-messenger", id: 310633997

###############################################################################
# 1. Core Command‑Line Tools
###############################################################################

brew "git"
# Industry-standard distributed version control system (DVCS).
# Use `git clone <repo>`, `git branch`, `git checkout`, `git merge`, `git push`
# to track changes, branch features, and collaborate with others.

# brew "wget"
# CLI utility for downloading files and entire sites.
# Supports recursive download (`wget -r`) and resume (`wget -c`).
# Great for mirroring docs or grabbing remote assets in scripts.

brew "curl"
# Versatile data-transfer tool.  
# Use `curl -X GET https://api.example.com` for quick API tests,
# or `curl -O http://example.com/file.zip` to download files.

# brew "htop"
# Interactive process viewer with colored CPU, memory, and I/O bars.
# Launch with `htop` to spot runaway processes and monitor resource usage.

# brew "tree"
# Recursively print directory structure in a tree-like format.
# `tree -L 2` limits depth for quick overviews of nested projects.

# brew "tmux"
# Terminal multiplexer: manage multiple panes/sessions in one window.
# Commands: `tmux new -s dev`, detach with Ctrl‑B D, reattach `tmux attach`.
# Ideal for long-running tasks (logs, servers) you can disconnect from.

###############################################################################
# 2. Shell & Terminal Enhancements
###############################################################################

# cask "iterm2"
# Replacement for Terminal.app: tabs, splits, custom profiles, hotkeys.
# Use Profiles → Send Text on Start to auto-run commands per project.

# brew "oh-my-zsh"
# Framework for managing zsh configuration with themes & plugins.
# Customize `~/.zshrc`, enable plugins like git, docker, npm for auto-complete.

# brew "zsh-autosuggestions"
# Suggests commands from history as you type.  
# Add `plugins+=(zsh-autosuggestions)` to `~/.zshrc` and restart shell.

# brew "zsh-syntax-highlighting"
# Highlights valid commands vs. typos in real time.
# Source in `~/.zshrc`: `source /usr/local/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh`.

# brew "starship"
# Lightning-fast, highly-customizable prompt written in Rust.
# Configure via `~/.config/starship.toml`; shows git status, language versions, time.

# brew "fzf"
# Fuzzy finder for the terminal.
# Install key bindings: `$(brew --prefix)/opt/fzf/install`.
# Use Ctrl‑T to fuzzy-open files, Ctrl‑R to search command history.

# brew "ripgrep"
# Ultra-fast recursive search (grep replacement).
# Example: `rg TODO` to find all TODO comments in your codebase instantly.

# brew "bat"
# `cat` clone with syntax highlighting and line numbers.
# Use `bat src/main.py` to view code with color and easier navigation.

# brew "fd"
# Simple, fast alternative to `find`.
# Example: `fd -e js import` to locate JS files containing “import”.

# brew "jq"
# Command-line JSON processor.
# Pipe API responses: `curl -s http://api.com | jq '.items[] | {id, name}'`.

###############################################################################
# 3. Programming Languages & Version Managers
###############################################################################

# brew "pyenv"
# Python version manager: isolate projects with different interpreters.
# `pyenv install 3.10.9`; in project: `pyenv local 3.10.9`; install packages via pip.

# cask "miniforge"
# ARM-optimized conda distribution.
# `conda create -n ml python=3.10`; `conda activate ml`; install TF/PyTorch inside.

# brew "nvm"
# Node.js version manager.
# After install, add to `~/.zshrc`: 
#   export NVM_DIR="$HOME/.nvm"
#   [ -s "$(brew --prefix nvm)/nvm.sh" ] && \. "$(brew --prefix nvm)/nvm.sh"
# Use `nvm install 18`, `nvm use 18`.

# brew "yarn"
# Fast JS package manager with deterministic installs.
# Use `yarn init`, `yarn add react`, and Yarn Workspaces for mono-repos.

# brew "rbenv"
# Ruby version manager.
# `rbenv install 3.2.2`; `rbenv global 3.2.2`; manage gems per version.

# brew "go"
# Google's statically-typed, compiled language.
# `go mod init myapp`; `go build ./...` to compile; `go fmt` to format code.

# brew "rustup-init"
# Rust toolchain installer.
# Run `rustup-init`, then use `cargo new` to scaffold new projects and `cargo build --release`.

cask "flutter"
# UI toolkit for cross-platform mobile, web, and desktop.
# `flutter create my_app`; `flutter run` to launch on simulators/emulators.

###############################################################################
# 4. Editors & IDEs
###############################################################################

cask "visual-studio-code"
# Extensible editor: install extensions like Python, ESLint, Prettier, Live Share.
# Use Settings Sync to keep your config across machines.

cask "android-studio"
# Official Android IDE: built-in emulator, SDK manager, code templates.
# Manage Android SDK versions in Tools → SDK Manager.

# cask "intellij-idea-ce"
# JetBrains IDE for Java, Kotlin, and web frameworks.
# Smart refactoring, built-in Docker & database tools.

# cask "jetbrains-toolbox"
# Central hub for installing/updating JetBrains IDEs.
# Auto-updates and easy rollback to previous versions.

# brew "neovim"
# Modern Vim with built-in LSP support and async plugins.
# Configure via `~/.config/nvim/init.lua`; use plugin managers like Packer.

# brew "emacs"
# Highly extensible editor with Org-mode, Magit, and countless packages.
# Launch GUI or `emacs -nw` for terminal mode.

###############################################################################
# 5. Build Tools & Libraries
###############################################################################

# brew "cmake"
# Cross-platform build system.
# Example: `cmake -S . -B build && cmake --build build` for out-of-source builds.

# brew "gcc"
# GNU Compiler Collection for C/C++.
# Compile C: `gcc hello.c -o hello`; compile C++: `g++ main.cpp -o app`.

# brew "autoconf"
# Generate portable `configure` scripts for Unix builds.
# Typical flow: `autoconf && ./configure && make && make install`.

# brew "automake"
# Generates Makefile.in scaffolding for projects using Autotools.

# brew "pkg-config"
# Utility to retrieve compiler and linker flags for libraries.
# Example: `pkg-config --cflags --libs libyaml`.

# brew "openssl"
# TLS/SSL library for secure communications.
# Link flags: `-I$(brew --prefix openssl)/include -L$(brew --prefix openssl)/lib -lssl -lcrypto`.

# brew "libyaml"
# Fast YAML parser, required by many Ruby/Python gems for YAML support.

# brew "libffi"
# Foreign Function Interface library, enables calling C functions from high-level languages.

###############################################################################
# 6. Containers & Orchestration
###############################################################################

# cask "docker"
# Container platform with GUI dashboard.
# `docker-compose up` to run multi-container apps declared in docker-compose.yml.

# brew "colima"
# Lightweight alternative to Docker Desktop on macOS.
# Start with `colima start --cpu 4 --memory 8`.

# brew "kubectl"
# Kubernetes CLI for managing clusters.
# `kubectl apply -f deployment.yml`; `kubectl logs pod-name`.

# brew "kind"
# “Kubernetes in Docker” for local cluster testing.
# `kind create cluster --name dev`.

# brew "minikube"
# Single-node local Kubernetes.
# `minikube start --driver=hyperkit`; `minikube dashboard`.

# brew "virtualbox"
# Virtual machine manager for running full OS images.
# Good for testing Linux/Windows environments or legacy software.

###############################################################################
# 7. Databases & Data Stores
###############################################################################

# brew "postgresql"
# Advanced open-source relational database.
# `brew services start postgresql`; use `psql` to create databases & run SQL.

# brew "mysql"
# Popular relational database, common in LAMP stacks.
# `brew services start mysql`; `mysql -u root` to access.

# brew "redis"
# In-memory key/value store and message broker.
# `brew services start redis`; connect via `redis-cli`.

# cask "mongodb-community"
# Document-oriented NoSQL database.
# `brew services start mongodb-community`; shell access with `mongo`.

# brew "sqlite"
# File-based SQL database engine.
# No server required—use `sqlite3 mydb.db` for quick prototyping.

###############################################################################
# 8. Web Servers & Proxies
###############################################################################

# brew "nginx"
# High-performance web server and reverse proxy.
# Config: `/usr/local/etc/nginx/nginx.conf`; reload: `brew services restart nginx`.

# brew "httpd"
# Apache HTTP Server.
# Config: `/usr/local/etc/httpd/httpd.conf`; reload: `brew services restart httpd`.

###############################################################################
# 9. Mobile Development Utilities
###############################################################################

brew "cocoapods"
# iOS dependency manager for Swift/Obj‑C libraries.
# `pod init`; define pods in Podfile; `pod install` to integrate into Xcode workspace.

# brew "carthage"
# Decentralized iOS/macOS dependency manager.
# `carthage update --platform iOS` to build frameworks you then embed manually.

# brew "fastlane"
# Automate builds, screenshots, code signing, and deployments.
# Define lanes in Fastfile, then run `fastlane beta` or `fastlane release`.

###############################################################################
# 10. Cloud & DevOps CLIs
###############################################################################

# brew "awscli"
# AWS Command-Line Interface.
# `aws configure` for credentials; `aws s3 cp file s3://bucket/` to upload.

# brew "azure-cli"
# Microsoft Azure management CLI.
# `az login`; create resources: `az group create`, `az webapp up`.

# brew "google-cloud-sdk"
# Google Cloud CLI tools (gcloud, gsutil, bq).
# `gcloud init`; deploy functions: `gcloud functions deploy`.

# brew "heroku/brew/heroku"
# Heroku CLI for managing apps & addons.
# `heroku login`; `heroku create` and `git push heroku main`.

# brew "gh"
# GitHub CLI for PRs, issues, releases.
# `gh auth login`; `gh repo create`; `gh pr review`.

# brew "azure-functions-core-tools"
# Local Azure Functions runtime.
# `func init MyFuncProj`; `func start` for local testing.

###############################################################################
# 11. AI & ML Frameworks & Helpers
###############################################################################

brew "jupyterlab"
# Browser-based interactive notebooks.
# Launch with `jupyter lab --notebook-dir=~/projects`.

# brew "opencv"
# Computer vision library for Python/C++.
# In Python: `import cv2`; use filters, feature detection, and video capture.

# brew "dvc"
# Data Version Control for ML pipelines.
# `dvc init`; `dvc add data.csv`; `dvc push` to remote storage.

# brew "mlflow"
# Experiment tracking & model registry.
# `mlflow ui` to visualize runs; integrate via `mlflow.log_metric`.

# brew "poetry"
# Python packaging & dependency manager.
# `poetry init`; `poetry add pandas`; auto-creates a virtualenv.

# brew "prefect"
# Workflow orchestration for data/ML tasks.
# Define flows in Python; deploy & schedule with `prefect`.

###############################################################################
# 12. Productivity & Miscellaneous Apps
###############################################################################

# cask "slack"
# Team messaging service with integrations.
# Connect GitHub, Jenkins, or custom bots for real-time alerts.

# cask "postman"
# API development environment.
# Organize requests into Collections; write JavaScript tests; export environments.

# cask "rectangle"
# Keyboard-driven window management.
# Snap windows to halves, thirds, or custom sizes using configurable shortcuts.

# cask "raycast"
# Productivity launcher & command bar.
# Search files, trigger scripts, manage TODOs, and integrate with many services.

###############################################################################
# 13. Requested Desktop Apps
###############################################################################

# cask "cursor"
# AI-powered coding assistant for VS Code & JetBrains.
# Generates code snippets, autocompletes functions, and fetches docs inline.

cask "google-chrome"
# Chromium-based browser with powerful DevTools & Lighthouse audits.
# Use profiles to segment work/personal environments.

# cask "firefox"
# Open-source browser with advanced privacy and developer tools.
# Use Responsive Design Mode and Network Performance inspector.

cask "spotify"
# Music streaming client.
# Keep your focus playlists at your fingertips; control from media keys or Raycast.

cask "discord"
# Voice, video, and text chat for communities.
# Join dev channels, get real-time help, and integrate bots for notifications.


cask "chatgpt"
# Native ChatGPT client for macOS.
# Drag-and-drop code snippets for instant AI-driven explanations and refactors.

