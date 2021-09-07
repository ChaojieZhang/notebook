# Linux commands

## add a sudo user

add user

```sh
adduser usernmae
```

add user to sudo group

```sh
usermod -aG sudo username
```

## ssh keygen

```sh
 ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

## command line vi mode

```sh
set -x vi
```

## vnc

```sh
apt-get install vino
```

solve vnc version not match error using macos

```sh
gsettings set org.gnome.Vino require-encryption false
```

## NCurses Disk Usage [link](https://dev.yorhel.nl/ncdu)

find out which folder is too big

```sh
ncdu
```