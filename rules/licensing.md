---
title: Licensing
layout: page-with-sidebar
tagline:
group: rules
---

###Requirements
*The requirements for licensing of resources*

###Discussion

The licensing of resources will impact how they can be shared.

####Licensing and Aggregation

Importantly licensing may affect whether resources can be shared directly as part of a serialization like a research object bundle, or whether they can only be referenced as part of a description like the research object manifest description.  

Consider for example the inclusion of the article text of an existing publication, as is done in the [clinical codes research object](https://github.com/CHIP-SET/clinicalcodes.article5). The associated publication "Withdrawing performance indicators: retrospective analysis of general practice performance under UK Quality and Outcomes Framework" - (dx.doi.org/10.1136/bmj.g330) has been published as an open access article. We are therefore able to serialise the pdf itself as part of the research object bundle, and include it in the manifest as follows:

     "aggregates" : [
     {
      "uri" : "http://dx.doi.org/10.1136/bmj.g330",
      "bundledAs" : {
        "filename"  : "/bmj.g330.pdf"
        "proxy" : "urn:uuid:83a3d644-b44a-42b2-b766-8cb269ec3f28"
      }
    },
    ...

If the article's copyright had instead been retained by the publisher, we would be restricted to only providing a URI pointing to the publication and not including the pdf.

###Examples
