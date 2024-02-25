# Web-Technology
# Installing Apache
    sudo apt update
    sudo apt install apache2
# Adjusting the Firewall
    sudo ufw app list
    sudo ufw allow 'Apache'
    sudo ufw status
# Checking your Web Server
    sudo systemctl status apache2
ctrl x
y
enter
# Setting up a single virtual host

    cd /etc 
    ls
    sudo nano hosts
     cd apache2
     cd sites-available
     sudo nano example.com.conf
     sudo a2ensite example.com.conf
     systemctl reload apache2
     sudo apache2ctl configtest
      sudo nano index.html 







