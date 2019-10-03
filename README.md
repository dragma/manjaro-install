# manjaro-install

**upgrade to last kernel first**

```console
# update all packages
sudo pacman -Syu
# install pacman packages
sudo pacman -S yay htop docker docker-compose devtools filezilla thunderbird peek jdk8-openjdk base-devel kolourpaint sshpass bluez bluez-utils
# configure docker
sudo systemctl start docker
sudo systemctl enable docker
sudo usermod -aG docker $USER
# update makepkg configuration
# => https://www.reddit.com/r/archlinux/comments/3ctiou/lpt_speed_up_makepkg_by_skippingparallelizing/
# install yay packages
yay -S spotify google-chrome visual-studio-code-bin redis-desktop-manager gitkraken android-studio robo3t-bin
# install nvm
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
```

Configure ANDROID_HOME in .bashrc
```
export ANDROID_HOME=~/Android/Sdk
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools
```
Accept android licences
```console
~/Android/Sdk/tools/bin/sdkmanager --licenses
```
install node & npm basic global packages
```console
nvm i 10.16.3
npm i -g npm eslint yarn pm2 expo-cli prisma react-native-cli

```
crack gitkraken
```console
mkdir ~/dev
cd ~/dev
git clone https://github.com/5cr1pt/GitCracken gticracken
cd gticracken/GitCracken/
yarn
yarn build
sudo yarn start patcher
```
```
