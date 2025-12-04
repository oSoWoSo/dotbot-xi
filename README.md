# Dotbot xbps Plugin

For use with [dotbot](https://github.com/anishathalye/dotbot),
this plugin allows one to easily install or upgrade a list of xbps packages
on Void Linux.

This plugin is recreation of
[xbps](https://github.com/m-wynn/dotbot-xbps) plugin, to use `xi` command instead  
(xi is part of xtools)

## Usage

Add this plugin to your dotfiles repo as a submodule

```bash
git submodule add https://github.com/oSoWoSo/dotbot-xi
```

```bash
./install -p dotbot-xi/xi.py -c install.conf.yaml
```

`xi` will handle raising privileges if needed.

Then, include the plugin and specify your desired packages in your `install.conf.yaml`:

```yaml
- plugins:
  - dotbot-xi/

- xi:
  - awesome
  - zsh
  - vim
```
