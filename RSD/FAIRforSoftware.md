# Open Science 

Open Science is an important part of out work at the NLeSC. We have open calls, we require open access papers, open data, and open source software, and a data management and software sustainability plan.

Where open access and open data are broadly accepted as an integral part of open science, open software is often forgotten or ignored. We feel open software is an essential part of open science. For most of research, software is an essential tool to produce the scientific results. Without the software, reproducing or extending existing work is hard if not impossible, even if the data and papers are open. 

Therefore, we feel research software should be open, just like research data and papers. However, simply producing open source software is not enough. As with open data simply providing a download link and permissive licence is only the start. As described in [The FAIR Guiding Principles for scientific data management and stewardship](https://www.nature.com/articles/sdata201618): 

_"Beyond proper collection, annotation, and archival, data stewardship includes the notion of ‘long-term care’ of valuable digital assets, with the goal that they should be discovered and re-used for downstream investigations, either alone, or in combination with newly generated data."_ 

## Why is software different from data ?

Although orginally indented for data, most of these principles also apply to research software. Like open data, we feel software should be FAIR, that is _Findable, Accessible, Interoperable, and Re-usable_. However, software is not simply data: 

- software is dynamic instead of static
- software requires a context to work (hardware, other software, data)
- software requires expertise to apply. Storing the software without storing this expertise does not makes sense. 
- like data, software contains errors. However, the effect of these errors in software have different effects than in data. For example, you cannot filter out "outliers" in software.
- software tends to age which makes archival and reproducability a problem. Hardware and software dependencies tend to change or disappear. 

Interestingly, data in itself does not age. Typically, problems with reading old data formats are caused software aging, but not by the data itself. 

## FAIR for data

From the FAIR website, FAIR for data stands for _Findable, Accessible, Interoperable, and Re-usable_.

In more detail:

__Findable:__ 

F1. (meta)data are assigned a globally unique and persistent identifier  
F2. data are described with rich metadata (defined by R1 below)  
F3. metadata clearly and explicitly include the identifier of the data it describes  
F4. (meta)data are registered or indexed in a searchable resource  
 
__Accessible:__

A1. (meta)data are retrievable by their identifier using a standardized communications protocol  
A1.1 the protocol is open, free, and universally implementable  
A1.2 the protocol allows for an authentication and authorization procedure, where necessary  
A2. metadata are accessible, even when the data are no longer available  

__Interoperable:__

I1. (meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation  
I2. (meta)data use vocabularies that follow FAIR principles  
I3. (meta)data include qualified references to other (meta)data  

__Reusable:__

R1. meta(data) are richly described with a plurality of accurate and relevant attributes  
R1.1. (meta)data are released with a clear and accessible data usage license  
R1.2. (meta)data are associated with detailed provenance  
R1.3. (meta)data meet domain-relevant community standards  

## Question: How to apply this to Software ? 

Below we translate the FAIR principles to software:

__Findable:__ 

F1. software is described with rich metadata (defined by R1 below) 
F2. metadata for software follows the FAIR principles as described above.
F2.1 this implies that metadata of software releases are assigned a globally unique and eternally persistent identifiers.  
   (implementation detail: releases should have a DOI, one globally for the software, and one per version)  
F2.2 this implies that metadata is registered or indexed in a searchable resource  
   (will be the RSD?)  
F3. metadata clearly and explicitly include the identifier of the software it describes  
   (links to the software and/or software releases?)  

Because metadata follows FAIR principles as stated above, the following only applies to the software it references. 

__Accessible:__

A1. The software is retrievable via the identifier contained in the metadata using a standardized communications protocol
   (for example, a URL, github link, etc).
A1.1 the protocol allows for an authentication and authorization procedure, where necessary  
A2. metadata are accessible, even when the software is no longer available  

__Interoperable:__

Idea: try to use standards (for example data formats, protocols and APIs) in the software. Use dependencies that follow the FAIR principles. 

I1. (meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation  
I2. (meta)data use vocabularies that follow FAIR principles  
I3. (meta)data include qualified references to other (meta)data  

__Reusable:__

R1. meta(data) are richly described with a plurality of accurate and relevant attributes  
    (authors, applications, locations of source, documentation, tutorials)   
R1.1. software is released with a clear and accessible usage license  
R1.2. software is associated with detailed provenance 
     (verion control)
R1.3. software meets domain-relevant community standards  
     (

## Misc decisions 

Metadata entries in the RSD have their own persistent unique identifier (like a DOI). The reason is that we do not control the repositories and releases of (all) the software in the RSD (like ROOT). We therefore do not control the DOIs (such as the ones generated by zenodo) that are stuck on a release. Having our own DOI for our own metadata and another one for the metadata in zenodo is not a problem. A drawback is that there are mutliple ways to cite something (via RSD-DOI or via Zenodo-DOI for example). This complicates the collection of metrics slightly. 





