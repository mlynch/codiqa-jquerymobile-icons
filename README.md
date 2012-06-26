Codiqa Icon Packs for jQuery Mobile
===================================

This project contains a growing set of icon packs meant for use in jQuery Mobile and other types of projects. Every icon pack comes with a regular and 2x size sprite sheet that supports high density displays (like iOS retina).

Read more about these icons here: http://blog.codiqa.com/2012/06/announcing-new-icon-packs-for-awesome-app-designs/

Unless specified otherwise, all icon packs are licensed under the [Creative Commons Attribution-ShareAlike 3.0 Unported](http://creativecommons.org/licenses/by-sa/3.0/) license. This means you are free to use these icon packs in both commercial and non-commercial settings, but you must attribute [Codiqa.com](http://codiqa.com/) and share any derivative works under the same or a similar license. All we ask is a link back to codiqa.com indicating that we provided the original version of the icons.

Usage in jQuery Mobile Apps
===========================

jQuery Mobile expects icons to be in 18x18 size. Several of our icon packs are larger and will not fit in very well without modifying the jQuery Mobile default CSS styles, so we have started to experiment with changes to jQuery Mobile that will support larger icon sizes.

You may have noticed that the `jquerymobile-style.css` stylesheet that comes with each pack contains some modifications to default jQuery Mobile styles. Always include these styles after importing the jQuery Mobile css. We have added a new field class `.ui-iconsize-N` that specifies the size of one dimension of a square icon. So, if your icons are 26x26 pixels, The `.ui-iconsize-26` class should be added to any icon element.

Unfortunately, we have only been able to hard-code sizes for 26x26 pixel icons, since that is what our first icon pack supports. Also, we are going to be experimenting and contributing changes to the jQuery Mobile javascript to handle the `data-iconsize` property of components that support icons. 
