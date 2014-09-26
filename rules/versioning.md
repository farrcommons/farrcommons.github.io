---
title: Versioning
layout: page-with-sidebar
tagline:
group: rules
---


###Requirements

*The requirements for versioning of resources*

###Discussion

Versioning concerns the versioning of individual resources, and versioning of a collection of resources.

#### Versioning of Resources

If you need to share a specific version of a resource, then this may be impacted by the identity mechanism, or whether that resource is under your stewardship.

Consider for example what resource is identified by the URL for the json-ld specification:

http://www.w3.org/TR/json-ld/

This URL will always resolve to latest version of the spec. Alternatively the following URL identifies a specific version of the specification:

http://www.w3.org/TR/2014/REC-json-ld-20140116/

Another approach to versioned resources is through the use of Momento which supports the retrival of previous versions of web resources, allowing for content negotiation based upon a time stamp.

Alternative approaches may need to be taken when the resource is not under your stewardship, and there is no versioned URI scheme.


####Versioning of Collections

###Examples
