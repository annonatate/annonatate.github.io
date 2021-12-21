---
title: Finding IIIF images
layout: default
nav_order: 11
---


<script src="{{site.baseurl}}/js/custom-search.js"></script>

<link rel="stylesheet" type="text/css" href="{{site.baseurl}}/css/custom-search.css">

# {{page.title}}

* TOC
{:toc}

## Please feel free to contribute to this page by opening an [issue](https://github.com/dnoneill/annotate/issues/new?assignees=dnoneill&labels=&template=add-resource-to--where-to-find-iiif-.md&title=)

# Tools
* [https://github.com/2SC1815J/open-in-iiif-viewer](https://github.com/2SC1815J/open-in-iiif-viewer) is "a Firefox/Chrome extension to open IIIF manifest link in your favorite IIIF viewer".


# Internet Archive

Images in the Internet Archive accessible through a IIIF endpoint. Instructions are located here: [https://medium.com/@aeschylus/use-internet-archives-iiif-endpoint-to-unlock-your-images-potential-9b0a3efa5b55](https://medium.com/@aeschylus/use-internet-archives-iiif-endpoint-to-unlock-your-images-potential-9b0a3efa5b55) or via [IIIF Guides](https://iiif.io/guides/guides/archive.org/).

# [WikiData](https://commons.wikimedia.org/wiki/Commons:International_Image_Interoperability_Framework)

Images in Wikidata can each have a manifest. They can be loaded in [https://tools.wmflabs.org/wd-image-positions/](https://tools.wmflabs.org/wd-image-positions/). For example the Item ID for this page: [https://www.wikidata.org/wiki/Q328523](https://www.wikidata.org/wiki/Q328523) is Q328523. The property ID should be P18 (this is Wikidata's image property).  The `Preview IIIF` will load the manifest into a Mirador instance. The `IIIF manifest` will be load the manifest and often there is a annotation list which may be empty. An example with annotations is [https://tools.wmflabs.org/wd-image-positions/item/Q1231009](https://tools.wmflabs.org/wd-image-positions/item/Q1231009). Here is the link to the manifest: [https://tools.wmflabs.org/wd-image-positions/iiif/Q1231009/P18/manifest.json](https://tools.wmflabs.org/wd-image-positions/iiif/Q1231009/P18/manifest.json). These manifests can not be loaded into the Mirador instance on this site without being changed however Wikidata image position tool allows for crowd sourced annotations. In order to get the manifest to work in this site's Mirador instance change `https://upload.wikimedia.org/wikipedia/commons/1/1e/Jacques-Louis_David_-_The_Coronation_of_Napoleon_%281805-1807%29.jpg` in the manifest to `https://tools.wmflabs.org/zoomviewer/proxy.php?iiif=Jacques-Louis_David_-_The_Coronation_of_Napoleon_%281805-1807%29.jpg/full/full/0/default.jpg` or load image into [Create annotations on IIIF images without a manifest]({{site.baseurl}}/openseadragon/) using method in  [Wikipedia Commons images](#wikipedia-commons-images).


# [Wikipedia Commons images](https://commons.wikimedia.org/wiki/Commons:International_Image_Interoperability_Framework)

In addition to images hosted on IIIF servers, Wikipedia Commons images can be loaded into a IIIF format using a static url. The Wikipedia Commons image filename is loaded into the URL below and the IIIF image will render.

```
https://tools.wmflabs.org/zoomviewer/proxy.php?iiif={image filename}/full/full/0/default.jpg
https://tools.wmflabs.org/zoomviewer/proxy.php?iiif={image filename}/info.json
```

## Examples
[https://tools.wmflabs.org/zoomviewer/proxy.php?iiif=Godward_Idleness_1900.jpg/full/full/0/default.jpg](https://tools.wmflabs.org/zoomviewer/proxy.php?iiif=Godward_Idleness_1900.jpg/full/full/0/default.jpg)

[https://tools.wmflabs.org/zoomviewer/proxy.php?iiif=The_Garden_of_Earthly_Delights_by_Bosch_High_Resolution.jpg/info.json](https://tools.wmflabs.org/zoomviewer/proxy.php?iiif=The_Garden_of_Earthly_Delights_by_Bosch_High_Resolution.jpg/info.json)

# [Wikidata with IIIF manifests](https://commons.wikimedia.org/wiki/Commons:International_Image_Interoperability_Framework)
Additionally a number of Wikidata entries have a manifest listed in the entry. This [Wikidata query link](https://query.wikidata.org/#%23artworks%20on%20Wikidata%20which%20link%20to%20IIIF%20manifests%0ASELECT%20%3Fitem%20%3FitemLabel%20%3Fcollection%20%3FcollectionLabel%20%3Fiiif_manifest%20%3Fcreator%20%3FcreatorLabel%20%3Finception%20WHERE%20%7B%0A%20%20%3Fitem%20wdt%3AP6108%20%3Fiiif_manifest.%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22%5BAUTO_LANGUAGE%5D%2Cen%22.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP195%20%3Fcollection.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP170%20%3Fcreator.%20%7D%0A%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP571%20%3Finception.%20%7D%0A%7D) provides the framework for viewing all Wikidata that links to a manifest. In order to view the results click on the play symbol. It does take a minute to load.

# ContentDM images

Search any image in ContentDM. [https://researchworks.oclc.org/iiif-explorer/](https://researchworks.oclc.org/iiif-explorer/)

# Search Academic repositories

<form role="search" id="search">
<div class="search-control">
    <input type="search" id="keyword" name="query"
           placeholder="Keyword Search"
           aria-label="Search institutions">
    <input type="hidden" name="sort" value="atoz">
</div>
</form>
<div id="spinner"><i class="fa fa-spinner fa-spin"></i></div>

<div id="header_info"></div>
<div style="float: left; width: 20%; ">
  <div id="facets">
  </div>
</div>
<div style="float: left; width: 80%; display: none; border: 1px solid #ccc" class="all_results">
  <div id="search_results">
    <div id="searchInfo">
      <span id="number_results"></span>
      <span id="sort_by" class="dropdownsort"><label for="sortSelect">Sort By:</label>
        <select id="sortSelect" name="sort" onchange="changeSort(event);">
          <option value="">Relevance</option>
          <option value="atoz">Name</option>
        </select>
      </span>
    </div>
  </div>
  <ul id="resultslist">
  </ul>
  <div id="pagination"></div>
</div>
<div style="clear:both"><span></span></div>
<script src="{{site.baseurl}}/js/index.js"></script>

<script type="text/javascript">
    function load() {
      const queryString = window.location.search;
      var newUrl = window.location.href;
      if (!queryString){
        document.getElementById('search').submit();
      } else if (queryString != '?query=&sort=atoz'){
        var addTo = window.location.href.indexOf('#search-academic-repositories') == -1 ? '#search-academic-repositories' : '';
        if (queryString.indexOf('query') == -1){
          newUrl = newUrl.replace('?', '?query=&');
        }
        if (addTo || newUrl != window.location.href){
          window.location.href = newUrl + addTo;
        }
      }
      
      loadsearchtemplate();
      document.getElementById('spinner').style.display = 'none';
      }
      window.onload = load;
</script>
