MTX9250 CPS patch for 900 MHz ham band

The Motorola Professional Trunking CPS needs modifications to cps_95nt.exe in
order to program channels in on the 900 MHz ham band.  There is no registry
hack for this software.

The files here were made using bsdiff and are binary patch files that can be
applied using bspatch from the same project.

If you are on Linux or otherwise have access to Linux, just try to install
bsdiff using your package manager.  It's probably available.  On Windows, you
can ge tit from Cygwin.  Here is the main site:

    http://www.daemonology.net/bsdiff/

In case you don't have bsdiff and can no longer find it on the Internet -or- if
you have a version of MTX9250 CPS that is not R02.03 nor R02.01.03, then you
may need to make the modification manually.  Do that by first making a backup
of cps_95nt.exe.  Then open cps_95nt.exe in a hex editor.  Change all
occurrences of:

    9428 BB37

To:

    D410 6835

Save the file and you should be good to go.
