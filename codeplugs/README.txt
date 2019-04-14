Code Plugs
----------

This directory structure is organized in a way to keep track of both users
and radio types.  The majority of things in here are for Motorola radios,
but the occassional non-Motorola radio may show up.

Here's the layout of the tree:

     +
     |
     +-- README.txt          This file
     |
     +-- originals/          Original code plugs saved before altering
     |                       things.  Filenames match radio serial numbers.
     |
     +-- <callsign>/         The end user's call sign.  Usually ham, but
         |                   could be GMRS or another service.
         |
         +-- <model>         The radio model and band (if required).  For
                             example, HT1250-VHF means the Motorola HT1250
                             model covering the VHF split.  But then DJ-G29
                             means the Alinco DJ-G29 radio which is only a
                             220 MHz/900 MHz ham radio.

Within the subdirectory you will then find code plug files.  Filenames are
all over the place, but try to give some sort of description and date stamp.
There's no real "latest" code plug in a generic sense, it's really more per
use case.
