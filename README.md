Cos' è?
È un pannello di controllo per terminale Linux

A cosa serve?
serve ad utilizzare un terminale tipo termux(si installa su android) e terminale Linux tipo: Debian, Arch, Fedora ecc ...

È possibile creare cartelle, file, gestire i permessi delle cartelle e dei file, condividere file e cartelle, condividere il progetto stesso, perché esso stesso è un file
È possibile anche installare pacchetti in modo facile, rendere il proprio dispositivo un: NAS, Server SSH, Server VNC, Server IoT

Perché l' ho creato?

Per cercare di facilitare l'utilizzo del terminale

Come si installa il progetto:

PER TERMUX:
scarica il file elenco e mettilo nella cartella Download del telefono

Poi installa Termux da qui:
https://f-droid.org/repo/com.termux_1002.apk

Ed infine copia e incolla questo su termux e premi INVIO(rispondi alla domanda: y):

termux-change-repo && pkg update -y && pkg upgrade -y && pkg install fish -y && pkg install apt -y && termux-setup-storage && cat /storage/emulated/0/Download/elenco > /data/data/com.termux/files/usr/bin/menu && chmod +x /data/data/com.termux/files/usr/bin/menu && ~ && menu

Per aprire il progetto scrivi: menu


PER PC LINUX:
Per installare il progetto sul terminale Linux dei PC i sistemi operativi compatibili sono:

Arch Linux, Debian/Ubuntu, Fedora/Red Hat, openSUSE, Alpine e Void

PER ARCH LINUX

Scarica il file elenco e mettilo su Scaricati del PC

Poi sul terminale copia ed incolla questo:

sudo pacman -S fish --noconfirm && mkdir -p ~/.local/bin && cp -f ~/Scaricati/elenco ~/.local/bin/menu && chmod +x ~/.local/bin/menu && fish -c 'fish_add_path ~/.local/bin'

Per aprire il progetto scrivi: menu

PER DEBIAN/UBUNTU

Scarica il file elenco e mettilo su Scaricati del PC

Poi sul terminale copia ed incolla questo:

sudo apt update && sudo apt upgrade -y && sudo apt install fish -y && mkdir -p ~/.local/bin && cp -f ~/Scaricati/elenco ~/.local/bin/menu && chmod +x ~/.local/bin/menu && fish -c 'fish_add_path ~/.local/bin'

Per aprire il progetto scrivi: menu








