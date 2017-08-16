Sportify Install
================

Here you can find a build of Spotify for Linux. We are running this ourselves and we will try to make sure it keeps pace with its Mac and Windows siblings. However, this version is unsupported. You can tell us what you think and ask other users for help at The Spotify Community.

Spotify for Linux is released as a Debian package. Our aim is that it should work with the latest Long Term Support release of Ubuntu, but we will try to make it work for other releases of Ubuntu and Debian as well.

Installation
------------

Add the Spotify repository signing keys to be able to verify downloaded packages: ::

    sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys BBEBDCB318AD50EC6865090613B00F1FD2C19886 0DF731E45CE24F27EEEB1450EFDC8610341D9410

Add the Spotify repository: ::

    echo deb http://repository.spotify.com stable non-free | sudo tee /etc/apt/sources.list.d/spotify.list

Update list of available packages: ::

    sudo apt-get update

Install Spotify: ::

    sudo apt-get install spotify-client

