# illumos-smf-zones
Zones as SMF services, as detailed in my article on OI Wiki backed up at https://web.archive.org/web/20200428053251/https://wiki.openindiana.org/oi/Zones+as+SMF+services or https://github.com/jimklimov/illumos-articles/blob/master/articles/Zones%20as%20SMF%20services%20-%20OpenIndiana%20Wiki.mht?raw=true (as MHT archive, most browsers read that), and some time ago originally posted at http://wiki.openindiana.org/oi/Zones+as+SMF+services

Currently this includes all the code defined as part of the SMF manifests,
so nothing to install except registration of the two XMLs. See Wiki article
for more details, or consult the command-line help.

The most trivial setup automation with

````
cd bin
./zoneadm-smf install
````

should register the needed services and wrap all your existing zones into
individual services grouped as `svc:/system/zone-group:default`

For related trickery, please see also:

* https://github.com/jimklimov/illumos-articles
* https://github.com/jimklimov/illumos-splitroot-scripts
* https://github.com/jimklimov/illumos-smf-zfspools

...and loosely related by general theme:

* https://github.com/jimklimov/vboxsvc

Hope this helps,
Jim Klimov
