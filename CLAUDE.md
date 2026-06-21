# CLAUDE.md — surfn-arc-breeze

## Project overview

Standalone repo for the **Surfn Arc Breeze** icon theme, split out of the
`erikdubois/surfn` monolith. See [README.md](./README.md).

## Current state

Ships one theme: `usr/share/icons/Surfn-Arc-Breeze/`. Packaged as
`surfn-arc-breeze-icons-git` (recipe in `~/KIRO-PKG-BUILD-ICONS/surfn-arc-breeze-icons-git/`),
`depends=('breeze-icons')`.

## Patterns & decisions

- Theme dir PascalCase; repo/package lowercase. `icon-theme.cache` rebuilt by the pacman
  hook on install. Theme `Inherits=breeze,Sardi,Numix-Circle,Numix,Papirus,Moka,gnome,hicolor`
  — note it does **not** inherit base Surfn. Bash scripts follow the canonical Kiro template.
