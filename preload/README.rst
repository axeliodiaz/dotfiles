Installation
------------

Install preload & prelink: ::

    sudo aptitude install preload prelink

Configuration
-------------

Configure the options: ::

    -a: Apply prelink to all binaries following the prelink.conf configuration file.
    -m: Enables memory saving.
    -R: Assigns random addresses.

Execute prelink: ::

    sudo prelink -amR

Change the file: ::

    /etc/default/prelink

And set: ::

    PRELINKING=unknown

By: ::

    PRELINKING=yes

Add the next line into /etc/apt/apt.conf file (and create it if not exists): ::

    DPkg::Post-Invoke {"echo Ejecutando prelink, espere...;/etc/cron.daily/prelink";}

