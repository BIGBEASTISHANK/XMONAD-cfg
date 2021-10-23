#First use chmod and give permission to package-install.sh
chmod +x ./package-install.sh

#Now run it
./package-install.sh

#Search File
ls $HOME -a

#If you dont find .xmonad then create. If it is their skip this process
mkdir $HOME/.xmonad

#Copy and paste xpm folder and xmonad.hs file in .xmonad folder
cp -r xpm $HOME/.xmonad/ && cp xmonad.hs $HOME/.xmonad/

#Now setup xmobar, just copy and paste xmobar file in .config
cp -r xmobar $HOME/.config/

#Set .xinitrc file
cp .xinitrc $HOME/

#Now reboot and login then use command
startx

#Enjoy
