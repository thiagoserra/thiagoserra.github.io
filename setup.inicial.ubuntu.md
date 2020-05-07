# Setup básico ou post-install do Ubuntu 20.04

## Primeiro, excluir
    sudo apt purge thunderbird* rhythmbox firefox* hexchat
    sudo apt remove vim-tiny


## Atualizar
    sudo apt update
    sudo apt upgrade


## Instalar alguns softwares de uso corrente
    sudo apt install ubuntu-restricted-extras
    sudo apt install gnome-sushi flameshot
    sudo apt install mc htop ncdu neofetch

    sudo apt install speedtest-cli speedometer
    sudo apt install p7zip-full rar
    sudo apt install ntfs-3g exfat-fuse exfat-utils
    sudo apt install fonts-liberation fonts-inconsolata ttf-mscorefonts-installer
    sudo apt install git vim ctags
    sudo apt install build-essential

    sudo apt install audacity gimp inkscape pdfshuffler


## Instalar os pacotes do Latex
    sudo apt install texlive-extra-utils texlive-base texlive-lang-portuguese texlive-pictures texlive-fonts-extra texlive-fonts-recommended


## Instalacão do youtube-dl
    sudo curl -L https://yt-dl.org/downloads/latest/youtube-dl -o /usr/local/bin/youtube-dl
    sudo chmod a+rx /usr/local/bin/youtube-dl



