ansible-onmyzsh for Debian/Ubuntu
============

Ansible role for installing zsh and the ever awesome Oh My ZSH project on Debian/Ubuntu system.

## Overwrite Default Variables

The `vars/main.yml` file should contain your list of packages you want to install in order to override defaults found in `defaults/main.yml`.

```yml
---
OHMYZSH_PLUGINS:
  - bundler
  - gem
  - git
  - rake
  - ruby
  - rsync
  - sudo
  - systemd
  - ubuntu
  - tmux
  - zsh_reload
  - zsh-navigation-tools
ZSH_THEME: "ys"
```

Additionally, you can overwrite the variables as part of your playbook.

```yml
---
...
  vars:
    OHMYZSH_PLUGINS:
      - bundler
      - gem
      - git
      - rake
      - ruby
      - rsync
    ZSH_THEME: "ys"
...
```
