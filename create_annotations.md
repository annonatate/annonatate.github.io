---
title: Create Annotations
layout: default
nav_order: 3
---


# Creating annotations steps
1. Choose an image, manifest or use one of our default images. An example of a manifest you can use to input is: https://d.lib.ncsu.edu/collections/catalog/ua050_004_287336_20230811_86492/manifest.json.
2. Click on the `Add Image` button in the `My Images` section.
![]({{site.baseurl}}/images/create-1.png){:class="helpimage"}
3. Click on the `Use external image` button. If you want to mess around without a specific image, click on one of the demo images in the section below.
![]({{site.baseurl}}/images/create-2.png){:class="helpimage"}
4. Add the URL of the image or manifest you want.
![]({{site.baseurl}}/images/create-3.png){:class="helpimage"}
5. Choose from one the options that appears. 
* `Add to My Images`: it will add the image to `My Images` so it will continue to appear so you can use it.
* `Make Copy`: (This only appears if the URL is a manifest): This will create a copy of the manifest in your workspace. This is handy if you want your annotations list URLs added to your manifest automatically.
* `View`: will allow you to view the image in the annotation viewer without adding it to the `My Images` section.
![]({{site.baseurl}}/images/create-4.png){:class="helpimage"}
6. After you click on any of the three buttons the pop up will disappear and the `My Images` section will collapse. Click on the `+` icon to expand the `My Images` section. Click on one of the shapes in the toolbar.
![]({{site.baseurl}}/images/create-5.png){:class="helpimage"}
7. Drag your mouse over the section of the image you want to annotate. Enter any text, georeferencing and/or tags you want to sent and click `Save`.
![]({{site.baseurl}}/images/create-6.png){:class="helpimage"}
8. You have created your first annotation. In order to view the annotations you need to switch over to the `hand` icon in the toolbar and click on the annotation or use the `List View` to view all your annotations in a list.

# Tips
* There is a small bug where sometimes the shapes won't form. Reload the page and try again.
* You can change the links to preloaded manifests and images. Directions to do this are [Edit profile/preloads/uploads]({{site.baseurl}}/profile) page.
* Any images or manifests you upload will automatically be added to the homepage.
* You can link to manifests, images and specific canvases (if manifest loaded) for editing. The correct parameters are:
   *  `manifesturl` for manifests
   *  `imageurl` for images
   *  `canvas` for a specific canvas in a manifest.


**i.e.** 
[https://annonatate.fly.dev/?manifesturl=https://iiif.biblissima.fr/chateauroux/B360446201_MS0005/manifest.json&canvas=https://bvmm.irht.cnrs.fr/iiif/4490/canvas/canvas-981441](https://annonatate.fly.dev/?manifesturl=https://iiif.biblissima.fr/chateauroux/B360446201_MS0005/manifest.json&canvas=https://bvmm.irht.cnrs.fr/iiif/4490/canvas/canvas-981441)
[https://annonatate.fly.dev/?imageurl=https://repository.duke.edu/fcgi-bin/iipsrv.fcgi?IIIF=/nas/repo_deriv/hydra/multires_image/40/58/a6/28/4058a628-c593-463e-9736-8a821e178fee/info.json](https://annonatate.fly.dev/?imageurl=https://repository.duke.edu/fcgi-bin/iipsrv.fcgi?IIIF=/nas/repo_deriv/hydra/multires_image/40/58/a6/28/4058a628-c593-463e-9736-8a821e178fee/info.json)



