---
title: Create Annotations
layout: default
nav_order: 3
---


# Creating annotations walkthrough

<video id="video" controls preload="metadata" width="100%">
   <source src="{{site.baseurl}}/videos/creating_annotations.mp4" type="video/mp4">
   <track label="English" kind="subtitles" srclang="en" src="{{site.baseurl}}/videos/creating_annotations.vtt" default>
</video>

# Tips
* Remember to hold down the shift key when creating annotations.
* You can link to manifests, images and specific canvases (if manifest loaded) for editing. The correct parameters are:
   *  `manifesturl` for manifests
   *  `imageurl` for images
   *  `canvas` for a specific canvas in a manifest.
**i.e.** 
[https://annonatate.herokuapp.com/?manifesturl=https://iiif.biblissima.fr/chateauroux/B360446201_MS0005/manifest.json&canvas=https://bvmm.irht.cnrs.fr/iiif/4490/canvas/canvas-981441](https://annonatate.herokuapp.com/?manifesturl=https://iiif.biblissima.fr/chateauroux/B360446201_MS0005/manifest.json&canvas=https://bvmm.irht.cnrs.fr/iiif/4490/canvas/canvas-981441)
[https://annonatate.herokuapp.com/?imageurl=https://repository.duke.edu/fcgi-bin/iipsrv.fcgi?IIIF=/nas/repo_deriv/hydra/multires_image/40/58/a6/28/4058a628-c593-463e-9736-8a821e178fee/info.json](https://annonatate.herokuapp.com/?imageurl=https://repository.duke.edu/fcgi-bin/iipsrv.fcgi?IIIF=/nas/repo_deriv/hydra/multires_image/40/58/a6/28/4058a628-c593-463e-9736-8a821e178fee/info.json)

* You can change the links to preloaded manifests and images. Directions to do this are [Edit profile/preloads/uploads]({{site.baseurl}}profile) page.
* Any images or manifests you upload will automatically be added to the links.
