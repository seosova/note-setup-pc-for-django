#Setup PC for Django
---

##Initial settings

1. Setup git

        sudo dnf install git xclip
        git config --global user.name "Denis Savenko"
        git config --global user.email seosova@gmail.com
        git config --global core.editor gedit
        ssh-keygen -t rsa -b 4096 -C "seosova@gmail.com"
        ssh-add ~/.ssh/id_rsa

    *Add this key on github. Copy key and add on githubs's settings page.*

        xclip -sel clip < ~/.ssh/id_rsa.pub

