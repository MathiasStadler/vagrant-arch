# arch of vagrant

## detect next mirror

```bash
#install refector
sudo pacman -S refector

# found mirror
sudo reflector --verbose -c Germany -c Italy -c Netherlands --age 12 --protocol https --sort rate --save /etc/pacman.d/mirrorlist
# show mirror list
cat /etc/pacman.d/mirrorlist

```

## update arch all installed packages

```bash
sudo pacman -Syu
```

## install docker

```bash
sudo pacman -S docker
```

## start docker service

```bash
sudo systemctl start docker
```
