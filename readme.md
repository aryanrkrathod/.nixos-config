##  Setup

Clone the repository into your home directory:

```bash
git clone https://github.com/rn-rf/.nixos-config.git ~/.nixos-config
```
Change Username From rn to your nixos Username
Apply the configuration:

```bash
sudo nixos-rebuild switch --flake ~/.nixos-config#Utopia
```

This will:

* install all required system packages
* configure the desktop environment
* link dotfiles into their correct locations
* set up the complete user environment

---

###  Updating the system

After making changes, rebuild with:

```bash
sudo nixos-rebuild switch --flake ~/.nixos-config#Utopia
```

or use the alias:

```bash
utopia
```

Your system will update automatically with the new configuration.

---

##  Overview

This repository contains the complete system and user environment configuration for my NixOS setup.

It uses:

* **Nix flakes** for reproducibility
* **Home Manager** for user environment management
* **Hyprland** as the primary Wayland compositor
* **Waybar** for status bar
* **Modular configuration structure** for maintainability

---

##  Architecture

```
.nixos-config/
├── flake.nix
├── hosts/
├── modules/
├── home/
└── dotfiles/
```

---


##  License

Personal configuration. Use freely for inspiration.


**System Name:** Utopia
**User:** rn
**OS:** NixOS (flake-based)
**Compositor:** Hyprland
