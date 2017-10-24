carstick
========

This role copies music from the local machine to a USB drive for offline tunes in the
car.

Requirements
------------

This role requires Ansible 1.4 or higher and platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows.

    # Location of music library
    tunes_library: "/Volumes/Extra/MP3"

    # Where USB stick filesystems get mounted, e.g. /Volumes on OSX
    mount_home: "/Volumes"

    # Label of volume to copy to (probably passed on command line)
    carstick_name: "COOL_TUNES"

Dependencies
------------

None

License
-------

GPLv3

Author Information
------------------

John Gardner


