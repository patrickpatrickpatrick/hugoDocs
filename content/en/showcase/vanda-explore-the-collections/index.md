---

title: V&A Explore the Collections
date: 2021-06-04

description: "Collections online portal for the V&A Museum"

# The URL to the site on the internet.
siteURL: https://collections.vam.ac.uk 

# Add credit to the article author. Leave blank or remove if not needed/wanted.
byline: "[Digital Media Team](https://www.vam.ac.uk), Victoria & Albert Museum"

---

Explore the Collections (ETC) is the online portal for Victoria & Albert Museum's collection. It allows users to search for objects using a text query and then to refine their results by using facets. When a user has found an object they are looking for, they are then able to view the page of an object record. This not only includes information about the object and its history (such as description, images and maker) but also where an object is located within the museum and what articles or features have been written about the object.

A unique aspect of our collections which made development of ETC challenging is the sheer size of our collections. There are over one million records and we wanted to ensure that any object page - no matter how obscure - would load quickly. For our use case, most of the information we are presenting will remain static. If there any changes to object records then they can be staggered and pages do not need to be simultaneously updated. Furthermore due to the potential wide spread of requested pages, caching dynamically generated pages would yield little performance benefit. So therefore, we determined that using static pages would ensure the best performance.

The next issue was how to generate over one million pages. We needed a fast static site generator with powerful templating tools. This is where Hugo came in. With Hugo we can generate the pages for all of the objects in the collection in around an hour! Not only that but running Lighthouse on any object page results in a performance score of 100. Hugo's templating tools also made building with a component-oriented approach a very straight forward process. Overall Hugo surpassed our expectations and we would recommend it for any static page project.
