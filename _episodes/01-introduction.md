---
title: "Introduction"
teaching: 10
exercises: 5
questions:
- "1 Does FAIR data means open data?"
- "2 What are Digital Objects and Persistent Identifiers?"
- "3 Different types of PIDs"
objectives:
- "The participant will understand that the FAIR principles are fundamental for Sustainable Science."
- "The participant will learn what human and machine-friendly digital objects are."
keypoints:
- "FAIR means human and machine friendly data sources which aim for transparency in science and future reuse."
- "DOI (Digital Object Identifier) is a type of PID (Persistent Identifier)"
---


### 1. Does FAIR data means open data?

> No.    
> FAIR means human and machine-friendly data sources which aim for transparency in science and future reuse  
{: .objectives}

<img src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/00-2.png" alt="FAIR and Open Science" style="max-width: 120%; height: auto;">

> ## What does it mean to be machine-readable vs human-readable?  
> **Human Readable** “Data in a format that can be conveniently read by a human. Some human-readable formats, such as PDF, are not machine-readable as they are not structured data, i.e. the representation of the data on disk does not represent the actual relationships present in the data.”  
> **Machine Readable**
> “Data in a data format that can be automatically read and processed by a computer, such as CSV, JSON, XML, etc. Machine-readable data must be structured data. Compare human-readable. Non-digital material (for example, printed or hand-written documents) is not machine-readable by its non-digital nature. But even digital material need not be machine-readable. For example, consider a PDF document containing tables of data. These are definitely digital but are not machine-readable because a computer would struggle to access the tabular information - even though they are very human readable. The equivalent tables in a format such as a spreadsheet would be machine-readable. As another example, scans (photographs) of text are not machine-readable (but are human readable!) but the equivalent text in a format such as a simple ASCII text file can machine readable and processable.”
{: .prereq}

<br>
<img src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/fair2.png" alt="Machine Friendly DO">
<br>

> ## Machine friendly = Machine-readable + Machine-actionable + Machine-interoperable
> During this sourcebook, we will be using "Machine-readable" and "Machine friendly" interchangeably. We like the term "friendly" since it can also include "machine-actionability" and "machine-interoperability."
{: .prereq}


> ## Exercise - Level Medium 🌶🌶
> **Understanding the jargon of data "things"**
> Data collection varies depending the field of research, therefore the digital object that is discribed.
> - Task: Perform with your group a search of the following data "things" and discuss the meaning, similarity and differences of each one of them. 
> - Dataset  
> - Database  
> - Data collection  
> - Data type
> - Data model    
{: .challenge}

### 2. What are Digital Objects and Persistent Identifiers?

A **Digital Object** is a bit sequence located in a digital memory or storage that has, on its own, informational value. For example:  

- A Scientific Publication
- A Dataset
- A Rich Metadata file
- A README file containing Terms of use & Access Protocols

<br>
<img src="https://datascience.codata.org/articles/10.5334/dsj-2020-015/dsj-19-1127-g1.png/" alt="Digital Object Anatomy" weight=500 height=400>
<br>

> ## To learn more about FAIR Digital Objects
> > **FAIR Digital Objects: Which Services Are Required?** [(Schwardman, Ulrich 2020)](https://datascience.codata.org/articles/10.5334/dsj-2020-015/)
> > **FAIR Digital Object Framework Documentation** [(BdSS, Luiz Olavo 2020)](https://datascience.codata.org/articles/10.5334/dsj-2020-015/)
: 
{: .callout}

<br>

A **Persistent Identifier (PID)** is a long-lasting reference to a (digital or physical) resource:

- Designed to provide access to information about a resource even if the resource it describes has moved location on the web
- Requires technical, governance and community to provide the persistence
- There are many different PIDs available for many different types of scholarly resources, e.g. articles, data, samples, authors, grants, projects, conference papers, and so much more

<br>
<p align="center"><iframe width="900" height="600" src="https://en.wikipedia.org/wiki/File:FREYA-The-power-of-PIDs-V05-1.webm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></p>

*Video: The FREYA project explains the significance of PID: [LINK TO SOURCE](https://en.wikipedia.org/wiki/File:FREYA-The-power-of-PIDs-V05-1.webm)*

### Different types of PIDs

PIDs have community support, organisational commitment and technical infrastructure to ensure the persistence of identifiers. They often are created to respond to a community's needs. For instance, the International Standard Book Number or ISBN was created to assign unique numbers to books, is used by book publishers, and is managed by the International ISBN Agency. Another type of PID, the Open Researcher and Contributor ID or ORCID (iD), was created to help with author disambiguation by providing unique identifiers for authors. The [ODIN Project identifies additional PIDs](https://project-thor.readme.io/docs/project-glossary) along with [Wikipedia's page on PIDs](https://en.wikipedia.org/wiki/Persistent_identifier).

In [Episode 6 (Data Archiving)](https://maastrichtu-library.github.io/circular-research-data-bootcamp/05-data-archiving/index.html), you will explore one type of PID, the DOI (Digital Object Identifier), which is usually the standard PID for Datasets and Publications




> ## Exercise - Level Easy 🌶
> 1. arXiv is a preprint repository for physics, math, computer science and related disciplines. 
> 2. It allows researchers to share and access their work before it is formally published. 
> 3. Visit the arXiv new papers page for [Machine Learning](https://arxiv.org/list/cs.LG/recent). 
> 4. Choose any paper by clicking on the 'pdf' link. Now use <kbd>control</kbd> + <kbd>F</kbd> or <kbd>command</kbd> + <kbd>F</kbd> and search for 'HTTP'. Did the author use DOIs for their data?
> 
> > ## Solution
> > Authors will often link to platforms such as GitHub where they have shared their software, and/or they will link to their website hosting the data used in the paper. The danger is that platforms like GitHub and personal websites are not permanent. Instead, authors can use repositories to deposit and preserve their data and software while minting a DOI. Links to software sharing platforms or personal websites might move, but DOIs will always resolve to information about the software and/or data. See DataCite's [Best Practices for a Tombstone Page](https://support.datacite.org/docs/tombstone-pages).
> {: .solution}
{: .challenge}


#### DOIs are everywhere, examples:
- Resource IDs (articles, data, software, …)
- Researcher IDs
- Organisation IDs, Funder IDs
- Projects IDs
- Instrument IDs
- Physical sample IDs,
- DMP IDs…
- Media: videos, images, 3D models 


<script type="application/ld+json">
{
    "@context": "https://schema.org",
    "@type": "Course",
    "name": "Circular Research Data Bootcamp",
    "description": "This is the coursebook of the Circular Research Data Bootcamp. This coursebook is an Open Educational Resources following the FAIR and Open Science recommendations. A week-long summer camp training looking at real-world examples to achieve data sustainability following the FAIR principles of research data management. ",
    "version": "v1.0",
    "url": "https://doi.org/10.5281/zenodo.6974103",
    "license": "https://creativecommons.org/licenses/by/4.0/legalcode",
    "dateCreated": {
        "@type": "Date",
        "@value": "2022-08-01"
    },
    "datePublished": {
        "@type": "Date",
        "@value": "2022-08-08"
    },
    "inLanguage": {
        "@type": "Language",
        "name": "EN",
        "alternateName": "EN"
    },
    "keywords": [
        "Research Data Management",
        "Research Data Reuse",
        "Bootcamp",
        "Online Summer Camp",
        "FAIR",
        "FAIR Digital Objects"
    ],
    "creator": {
        "@type": "Person",
        "name": "concat @givenName @familyName",
        "givenName": "Pedro",
        "familyName": "Hernandez Serrano",
        "image": "https://avatars.githubusercontent.com/u/12054964?v=4",
        "jobTitle": "Data Steward",
        "email": "p.hernandezserrano@maastrichtuniversity.nl",
        "affiliation": {
            "@type": "Organization",
            "name": "Maastricht University Library",
            "url": {
                "@type": "URL",
                "@value": "https://library.maastrichtuniversity.nl/research/rdm/"
            }
        }
    },
    "contributor": [
        {
            "@type": "Person",
            "givenName": "Maria",
            "familyName": "Vivas Romero",
            "jobTitle": "Data Steward",
            "email": "m.vivasromero@maastrichtuniversity.nl",
            "affiliation": {
                "@type": "Organization",
                "name": "Maastricht University Library",
                "url": {
                    "@type": "URL",
                    "@value": "https://library.maastrichtuniversity.nl/research/rdm/"
                }
            }
        }
    ],
    "publisher": {
        "@type": "Person",
        "name": "Pedro Hernandez Serrano",
        "givenName": "Pedro",
        "familyName": "Hernandez Serrano",
        "jobTitle": "Data Steward",
        "email": "p.hernandezserrano@maastrichtuniversity.nl"
    },
    "citation": {
        "@type": "CreativeWork",
        "name": "Circular Research Data Coursebook",
        "creator": [
            {
                "@type": "Person",
                "name": "Pedro Hernandez Serrano"
            },
            {
                "@type": "Person",
                "name": "Maria Vivas Romero"
            }
        ]
    },
    "learningResourceType": "Coursebook",
    "provider": {
        "@type": "Organization",
        "name": "Maastricht University"
    }
}
</script>