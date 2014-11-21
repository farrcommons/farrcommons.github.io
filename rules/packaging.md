---
title: Packaging and Aggregation
layout: page-with-sidebar
tagline:
group: rules
---

###Requirements
*The requirements for packaging and aggregation of resources*

###Discussion

In many cases, to ensure that the data are maximally useful and reusable it is necessary to associate that data with related resources as collection.  

The ro bundle mechanism [\[Soiland-Reyes\]](https://w3id.org/bundle/) of serialisation is based upon a Zip archive that specialises the Adobe Universal Container Format. The ro bundle contains a manifest file that describes the aggregation. This manifest can refer to files that are part of the Zip archive, or simply refer to resources that are elsewhere via a URI.

Consider as well any restrictions of authorisation, and whether certain parts of the research object are restricted, and should only be accessible to certain people. In this case then it would be prefereable for the resources to remain hosted in their original location - so that authentication and authorization remains with the original data provider.
