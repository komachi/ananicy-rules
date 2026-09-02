# ananicy-rules

This is collection of [ananicy-cpp](https://gitlab.com/ananicy-cpp/ananicy-cpp) rules forked from [CachyOS collection of ananicy-rules](https://github.com/CachyOS/ananicy-rules).

Main difference is that this fork adds Debian-specific rules and rules for compilers, originally to be used for [ansible-decent-desktop](https://github.com/komachi/ansible-decent-desktop) project.

## Installation

```sh
sudo make install
```

This script will copy all the rules from this repo to `/etc/ananicy.d` dir.

## How to contribute

If your rule can be added to upstream collection maintained by CachyOS, [please open PR there](https://github.com/CachyOS/ananicy-rules). This fork backports rules from upstream.

If your rule is applicable only for Debian or it's a rule for a compiler, you can open PR here.

### Linting

```sh
make lint
```

This will check rules syntax and also check for duplicates. Script requires Python and [python-fastjsonschema](https://horejsek.github.io/python-fastjsonschema/) to be available.

Games can be sorted with `sort-games.sh`, for more information run this in terminal: `./sort-games.sh --help`

## How to find out proper process name?

Here is a list of tools

### CLI

- [htop](https://htop.dev/)
- [btop](https://github.com/aristocratos/btop)

### GUI

- System Monitor [KDE Plasma](https://apps.kde.org/plasma-systemmonitor/) or [GNOME](https://help.gnome.org/users/gnome-system-monitor/)

**Don't use absolute paths for the executables. Process name alone is enough.**
