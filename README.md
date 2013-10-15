## Preconditions
- Install 32bit compatible libraries if uder _64bit_ environment.
-- On fedora(redhat), the following packages are required:
--- glibc.i686
--- libXtst.i686

- Must have perl and perl/gtk.
-- On ubuntu, it's libgtk2-perl and libwww-perl
-- On redhat, its' perl-Gtk2
- Install 32bit oracle jdk, download it from oracal's web site.

## Configure steps
- Modify the junipernc script.
-- Change `export JDK_HOME=/path/to/your/sunjdk32/` to the right path
- Copy juniper binaries to right place
-- `mkdir ~/.juniper_networks`
-- `sudo cp -r juniper_networks/* ~/.juniper_networks`
-- `sudo chown -R han:han ~/.juniper_networks`
-- `sudo chown -R root:root ~/.juniper_networks/network_connect/ncsvc`
-- `sudo chmod u+s ~/.juniper_networks/network_connect/ncsvc`

## Run
- Execute `junipernc`.
-- The first run would give out some error messages, just ignore it and rerun.
