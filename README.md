mineque-osd-darkblue.xml
================

My own Navit layout based upon android-mdpi

You will probably need the svg icons from : https://github.com/twain47/Open-SVG-Map-Icons

Navit currently expects all icons to be in xpm/ so you need to rename them:
```bash
for d in *; do for f in $d/*; do mv $f ${d}_`basename $f`; done; done
```

Then move all icons to navit-src/navit/xpm/ and run make

To use this OSD and / or layout, just clone the code into your .navit folder and add these 2 lines in your navit.xml (right before your other OSD declaration is fine) :
```xml
<xi:include href="${HOME}/.navit/navit-osd-darkblue/mineque-osd-darkblue.xml"/>

```

This OSD currently looks like this :

![navit-nuc-darkblue](https://github.com/mineque/navit-osd-darkblue/raw/master/screenshot.png)
