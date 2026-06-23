# Changelog

## 2026.06.23 — README install commands

### What Changed

**Install docs:** the README install section now lists the meta packages (top-level `*-icons-meta`, plus the group meta where applicable) alongside the per-variant `*-icons-git` package — replacing the outdated single `pacman -S` line.

### Files Modified

- README.md

## 2026.06.21 — repo standardisation

### What Changed

Brought the standalone **Surfn-Arc-Breeze** repo in line with the other surfn theme
repos: relocated the icon tree to `usr/share/icons/`, corrected the README, and added
the standard project docs.

### Technical Details

- Icon theme moved from `surfn-icons/` to `usr/share/icons/Surfn-Arc-Breeze/`; the
  packaging recipe `surfn-arc-breeze-icons-git` (in `~/KIRO-PKG-BUILD-ICONS/`) was
  updated to copy from the new path.
- README dependency note corrected: the theme `Inherits=breeze,…` (not the base Surfn
  set), so the package depends on `breeze-icons`, not `surfn-icons-git`.
- Added CLAUDE.md.

### Files Modified

- usr/share/icons/Surfn-Arc-Breeze/ (relocated)
- README.md, CHANGELOG.md, CLAUDE.md
