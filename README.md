# RaspberryPi-Armduino
Script files to setup the RaspberryPi for using the Armduino board.

Installation:

Copy the three scripts, rc.function, rc.gpio and rc.teardown to /etc:

    sudo chmod +x rc.*
    sudo chown root.root rc.*
    sudo cp rc.* /etc

Copy the armduino script to /etc/init.d:

    sudo chmod +x armduino
    sudo chown root.root armduino
    sudo cp armduino /etc/init.d/

Setup the armduino script to run as a service:

    sudo update-rc.d armduino defaults
    sudo service armduino start

