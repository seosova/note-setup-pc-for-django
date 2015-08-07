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

2. Install python environment (for Fedora 22, python 3 default)

        sudo python3 -m pip install --upgrade pip
        sudo python3 -m pip install virtualenv

3. Create project

        mkdir ~/myproject
        cd ~/myproject
        virtualenv myprojectenv
        source myprojectenv/bin/activate
        pip install django psycopg2 nginx
        
        