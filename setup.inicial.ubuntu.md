# Setup básico ou post-install do Ubuntu 20.04
O que não está aqui:
  - Browser: [Vivaldi](https://vivaldi.com/pt-br/)
  - [Insync](https://www.insynchq.com)
  - [Ulauncher](https://ulauncher.io)

## Primeiro, excluir
    sudo apt purge thunderbird* rhythmbox firefox* hexchat
    sudo apt remove vim-tiny


## Atualizar
    sudo apt update
    sudo apt upgrade


## Instalar alguns softwares de uso corrente
    sudo apt install ubuntu-restricted-extras
    sudo apt install gnome-sushi flameshot
    sudo apt install mc htop ncdu neofetch curl

    sudo apt install speedtest-cli speedometer
    sudo apt install p7zip-full rar
    sudo apt install ntfs-3g exfat-fuse exfat-utils
    sudo apt install fonts-liberation fonts-inconsolata ttf-mscorefonts-installer
    sudo apt install git vim ctags
    sudo apt install build-essential apt-transport-https ca-certificates software-properties-common

    sudo apt install audacity gimp inkscape pdfshuffler


## Instalar os pacotes do Latex
_Mudar isso para o docker??_
    sudo apt install texlive-extra-utils texlive-base texlive-lang-portuguese texlive-pictures texlive-fonts-extra texlive-fonts-recommended


## Instalacão do youtube-dl
    sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
    sudo chmod a+rx /usr/local/bin/youtube-dl


## Docker
Para instalar:
    sudo apt install docker.io docker-compose

Depois:
    sudo systemctl enable --now docker

Depois:
    sudo usermod -aG docker thiago

Depois só checar:
    docker --version
