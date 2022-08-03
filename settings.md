---
title: Settings
layout: default
nav_order: 10
---

## Viewer
- options: default, mirador
- default option: default (Annotorious)
### What does this do
This allows you to choose which tool you want to use for annotating images. The default annotation tool is called Annotorious and it create W3 web annotations. The other option is Mirador2 which will give you an open annotation (older standar). 

We are currently looking at integrating Mirador3, however at the current time, Mirador3's annotations tools are not at a point where we can integrate them with our application.


## Tempuser
- options: notenabled, enabled
- default option: notenabled

### What does this do
This was built for our classroom instances. It allows for users to share a GitHub login and still have a specific identifiable username to be associated with the annotations create. When the user logs in, they are given a form they have to fill out with a unique temporary username they create for themselves.

## Widgets (only works with the default viewer)
- options: comment-with-purpose, comment, tag, geotagging
- default option: comment-with-purpose, tag, geotagging

### What does this do
This allows you to choose which fields show up on the default viewer. Currenlty we use 'comment-with-purpose' (see [Dropdown on creating annotation page](/purpose), the 'tag' (allows for the creation of tags), and 'geotagging' (allows for geotagging). This setting allows you to create a custom view. The view will be sorted by how you order these settings.
