## Getting started

```
git remote add aur ssh://aur@aur.archlinux.org/dbus-executor.git
git fetch aur
```

## Publishing

```
makepkg -g
# copy the SHA
makepkg
makepkg --printsrcinfo > .SRCINFO
# add and commit the things
git push aur main:master
```
