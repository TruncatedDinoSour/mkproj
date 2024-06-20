# This repository has been migrated to the self-hosted ari-web Forgejo instance: <https://git.ari.lt/ari/mkproj>
# Mkproj

> Make and use templates for projects

# Requirements

- Python 3.8 and up

# Installation

## Manual

```bash
sudo install -Dm0644 mkproj.1 /usr/share/man/man1/mkproj.1
sudo mandb -qf /usr/share/man/man1/mkproj.1
sudo install -Dm755 mkproj /usr/local/bin
```

## Packages

- Linux
  - Gentoo linux: [app-misc/mkproj::dinolay](https://ari-web.xyz/gentooatom/app-misc/mkproj)

# Customisation

Templates can be made and viewed in `~/.config/proj_tmpl` directory with a structure of

```
template_name/
    mkproj_autorun      -- A script that will run after initialising the template
    file1
    dir1/
        something
```

`mkproj_autorun` is a special file that will get auto-ran on project creation,
keep in mind that **having it is optional**

More in the `man` page
