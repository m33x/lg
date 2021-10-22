# LG webOS TV Tools

Only one tool here at the moment: a bash script to run on a rooted TV to update the recently expired LetsEncrypt CA certificates (useful for Plex or Emby setups that use LetsEncrypt certificates, since LG have not updated the CA certs on many TVs). You must have root on your TV. Once you have shell access, download this script with wget and run it.

On a rooted B9 or C9 you can open a shell on your TV and run the following four commands:

    cd /tmp
    wget https://raw.githubusercontent.com/tf318/lg/main/update-ca-certs.sh 2
    chmod +x update-ca-certs.sh
    ./update-ca-certs.sh


After updating the certs, the TV will reboot, and you should be good to go.

As I have no other LG devices on which to test this (filesystem layouts may be different), you may want to inspect the bash script and manually edit and run individual commands within instead, or at least use it as a guide for what to do on your own TV.
