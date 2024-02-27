# Web-Technology
# Check Ubuntu Version
    lsb_release -a
    lsb_release -r
    cat /etc/lsb-release

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
    Go to host and set the host name

  sudo nano /etc/hosts

    Create conf file

  sudo nano /etc/apache2/sites-available/example.com.conf

    Enable conf file

  sudo a2ensite example.com.conf

    Check config test

  sudo apache2ctl configtest

    Reload apache2

  systemctl reload apache2
  or, sudo systemctl restart apache2

    Create a sample index.html page using nano

  sudo mkdir -p /var/www/example.com/html
  nano /var/www/example.com/html/index.html







