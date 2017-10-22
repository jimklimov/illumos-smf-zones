# illumos-smf-zones
Zones as SMF services, as detailed in my article on OI Wiki
http://wiki.openindiana.org/oi/Zones+as+SMF+services

Currently this includes all the code defined as part of the SMF manifests,
so nothing to install except registration of the two XMLs. See Wiki article
for more details, or consult the command-line help.

The most trivial setup automation with

````
cd bin
./zoneadm-smf install
````

should register the needed services and wrap all your existing zones into
individual services grouped as svc:/system/zone-group:default

Hope this helps,
Jim Klimov
