---
title: Identity
layout: page-with-sidebar
tagline:
group: rules
---

###Requirements

*Requirements for the identification of resources*

1. Each unique research object placed into the Commons **must** have a unique identifier.

###Discussion

Research Objects are collections of one or more resources or "digital objects". Examples of these digital objects might be a data set, executable software, source code, or a pdf paper describing an investigation, as well metadata that describes those resources.

An identity mechanism is required for research objects, and the resources that they contain, for several reasons:

- **Citation:** To be able to talk unambiguously about either individual resources, or the research object so that we can **cite** them as **evidence**.
- **Location/Resolution:** To be able look up and retrieve those resources.
- **Credit** To be able to attribute a given resource to an individual, group, or organization.

A prevalent identity mechanism used in scholarly publishing is the Digital Object Identifier (DOI) scheme. As such we might expect that DOIs satisfy all requirements for identification of research objects. DOIs are have achieved a significant level community acceptance, and have established a broad infrastructure.  

Not all data are the same, and different identify mechanisms are suitable for different data.
The most important factor when it comes to citation is that the identifier should be **unambiguous** - that is, it should **uniquely** identify a specific resource.

A previous study by [Duerr2011][^1] investigating the utility of identification schemes in the earth sciences breaks the requirements for identifiers down further into 4 separate issues:

1. A **Unique Identifier**: To uniquely and unambiguously identify a particular piece of data, no matter which copy a user has.
2. A **Unique Locator**: To locate an authoritative copy of the data no matter where they are currently held
3. A **Citable Locator**: A combination of 1 & 2 to identify cited data.
4. A **Scientifically Unique Identifier**: To be able to tell that two data instances contain the same information even if the formats are different.

These 4 issues place increasingly

The final requirement for a "Scientifically Unique Identifier" highlights that there are requirements placed on identifiers in scholarship that not all identifier schemes can satisfy, including the DOI mechanism. Consider the case where we wish to know whether two articles are referring to the same research object, and they use DOIs. In a discussion of DOIs [Bilder 2013][^2] highlights that there are many examples of research artifacts with multiple DOIs, for example:

    http://dx.doi.org/10.6084/m9.figshare.91541

and

    http://dx.doi.org/10.1038/npre.2012.7151.1

If this is a particularly important requirement for a class of data, then a controlled identity scheme, or a deterministic identity scheme is required. [Thompson 2013][^3] discusses three features that define a controlled or "managed" identity scheme, *Syntax*, *Binding* and *Resolution*:

- *Syntax*: Constraints are placed on the form of names e.g:
• Country and language codes
• Domain names

- *Binding*: How a name gets (and maybe loses/changes) its meaning
• Some legislative process
• More-or-less explicit constitution of governing bodies

- *Resolution*: Given a name, how do you find out what it means?
• Official publications, a.k.a registries
• More-or-less well-defined search procedures
• Online lookup (bind, search engines)


The The IUPAC International Chemical Identifier (InChI) is what we might refer to as a *deterministic scheme* for the identification of chemical substances that can be used in printed and electronic data. That is the identifier is derived from the data such that same data will always have the same identifier. For example the identifier for the chemical aspirin is:

    InChI=1S/C9H8O4/c1-6(10)13-8-5-3-2-4-7(8)9(11)12/h2-5H,1H3,(H,11,12)  

The ability to provide such a determinisitc naming

The resource identification initiative builds upon existing vendor identification schemes and prescribes a verbose mechanism of citation

    "GeneTex Cat# GTX95689 RRID:AB_846382"

Which can be resolved at:

    http://antibodyregistry.org/search.php?q=AB_846382


###Resolution

Resolution is the process of taking an identifier and locating the **referent** - the resource to which the identifier refers.  

A standard http URI, e.g. http://www.w3.org/TR/webarch/ for example uses the existing Web architecture for the purposes of resolution.  

Some identity mechanisms such as PURLs, RRIDs and the DOI ecosystem provide a level of fault-tolerance in their resolution system, by having registries that associate a given PURL, RRID, or DOI with a URI on the Web.  This level of indirection provides some protection against issues of link decay on the web, allowing maintainers of the identifiers to update broken links with the registry.

An alternative to this is to make use of a Web Archiving initiative such as the the Web Archive (archive.org) or the UK Web Archive (http://www.webarchive.org.uk).


####Identity and Versioning

Research objects can be both individual resources, or a collection of a number of resources that make up an investigation.

When citing a resource we may wish to make either a *summary level* or *version level* citation.

If you need to talk about a specific version of a resource or research object, then this may be impacted by the identity mechanism, or whether that resource is under your stewardship.

Consider for example what resource is identified by the URL for the json-ld specification:

http://www.w3.org/TR/json-ld/

This URL will always resolve to latest version of the spec. If we wish to make a summary level citation of the json specification - making reference to the json spec in general - then this is sufficient.

Alternatively the following URL identifies a specific version of the specification:

http://www.w3.org/TR/2014/REC-json-ld-20140116/

### Representation ####
Resources will be requested and consumed by both people and machines.

When a human requests a resource, we should provide a human readable representation of that resource - for example a "splash page" describing a data collection.

When a machine requests a resource we should instead provide a machine readable representation of the resource.

<!--OAI-PMH?

If resources are
-->

### Recommended Formats ###

ORCID ids for identifying people
DOIs for identifying stable resources

### Examples###


###References###

[^1]:  Ruth E. Duerr et al., **On the utility of identification schemes for digital earth science data: an assessment and recommendations**

[^2]: Builder G., **DOIs unambiguously and persistently identify published, trustworthy, citable online scholarly literature. Right?** http://crosstech.crossref.org/2013/09/dois-unambiguously-and-persistently-identify-published-trustworthy-citable-online-scholarly-literature-right.html#comment-4983

[^3]: Henry S. Thompson., Naming on the Web: **What scholars should want, and what they can have** http://indico.cern.ch/event/211600/session/3/contribution/2/material/slides/0.pdf
