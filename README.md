# manjaro-install

**upgrade to last kernel first**

```console
# update all packages
sudo pacman -Syu
# install pacman packages
sudo pacman -S yay htop docker docker-compose devtools filezilla thunderbird peek jdk8-openjdk base-devel kolourpaint
# configure docker
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
# install yay packages
yay -S spotify google-chrome visual-studio-code-bin redis-desktop-manager gitkraken android-studio
# install nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```
