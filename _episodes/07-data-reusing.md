---
title: "Data Reusing"
teaching: 10
exercises: 15
questions:
- "1 How to cite data when reusing a data source?"
- "2 How do we make sure data will be reused?"
objectives:
- "The participant will understand the importance of data citation"
- "The participant will learn tools to test discoverability for data to be reused"
keypoints:
- 'Digital Objects (e.g. Datasets) "live" in the web, imagine they are like fishes in the sea 🐠🐠. The way to get picked up by a "fisherman" 🎣 i.e. a search engine (e.g. Google) is by describing these Digital Objects with Rich Metadata'
---

> ## FAIR principles used in Data Reusing:  
> **Findable**   
> > FM-F1B (Identifier persistence) → [doi.org/10.25504/FAIRsharing.TUq8Zj](https://doi.org/10.25504/FAIRsharing.TUq8Zj)  
> > FM-F4 (Indexed in a Searchable Resource) → [doi.org/10.25504/FAIRsharing.Lcws1N](https://doi.org/10.25504/FAIRsharing.Lcws1N)  
>
> **Reusable**  
> > FM-R1.2 (Detailed Provenance) → [doi.org/10.25504/FAIRsharing.qcziIV](https://doi.org/10.25504/FAIRsharing.qcziIV)  
>
{: .checklist}


## 1. How to cite data when reusing a data source?

> "Data Reusing" are activities for recycling existing research data sources.   
{: .objectives}
By default, we should make the research data documentation in citable and reusable formats    

The minimum citation elements recommended by [DataCite](https://datacite.org/) are:
- Creator
- Publication Year
- Title
- Resource Type or Version
- Publisher
- Digital Object Identifier

For example:

> Neff, Roni A.; L. Spiker, Marie; L. Truant, Patricia (2016): Wasted Food: U.S. Consumers' Reported Awareness, Attitudes, and Behaviors. PLOS ONE. Dataset. [https://doi.org/10.1371/journal.pone.0127881](https://figshare.com/articles/dataset/_Wasted_Food_U_S_Consumers_Reported_Awareness_Attitudes_and_Behaviors_/1445199) 
{: .prereq}

Original dataset at **Wasted Food: U.S. Consumers' Reported Awareness, Attitudes, and Behaviors** → [LINK TO EXAMPLE](https://figshare.com/articles/dataset/_Wasted_Food_U_S_Consumers_Reported_Awareness_Attitudes_and_Behaviors_/1445199) 

Nowadays, data repositories have a friendly interface on which one can export the data citation directly from the webpage. Such as ZENODO, Dataverse or FigShare.

<img src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/07-1.png" alt="cite">

> ## Citing datasets increases publication visibility on 25%.
> When we cite a dataset using a standard format (e.g. recommended DataCite), then we allow data aggregators to "pick up" on the citations just like publications. Therefore, they immediately become discoverable for scientific sources
> 
{: .callout}

## 2. How do we make sure data can be reused?

Remember that a dataset or a data source is a digital object. So Digital Objects "live" on the web. Imagine they are like fishes in the sea 🐠🐠. The way to get picked up by a "fisherman" 🎣 i.e. a search engine (e.g. Google), is by describing these Digital Objects with Rich Metadata [(Episode 5)](https://maastrichtu-library.github.io/qualitative-FAIR-data/06-rich-metadata/index.html). Moreover we can check the quality of discoverability of the Digital Objects by conducting automated tests.

There are different available applications to test the discoverability of datasets for future reuse.

For example:   
In **Google Rich Results** [search.google.com/test/rich-results](https://search.google.com/test/rich-results), you can test whether a dataset is discoverable by other machines (e.g. Google bots)→ [LINK TO EXAMPLE](https://search.google.com/test/rich-results/result?id=vQwCBt98I-8izEUmIVFQOQ)  

<img src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/07-2-II.png" alt="google" width="700" height="360">

After testing the URL of the data source, you will get the response from the Google bots. We aim to determine if the Google bots have found a structured dataset with the link we provided.

<img src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/07-3-II.png" alt="google2" width="700" height="470">

> ## Following the FAIR principles, you ensure Rich Metadata
> Rich metadata is necessary to be discoverable on the internet. Without testing it, your data can be virtually invisible on the web
> 
{: .callout}


> ## Exercise - Level Easy 🌶
>
> 1. The following website is a database of crime news related to cultural objects
> 2. Go to [news.culturecrime.org](https://news.culturecrime.org/all)
> 3. Perform Google's rich test on this data source 
> 4. You can copy the URL of the browser and put it on the [search.google.com/test/rich-results](https://search.google.com/test/rich-results)  
> **Question:** Did the Google bots find the dataset?
> {: .source}
>
> > ## Solution
> >
> > Nope 🙁  
> > They did not. This is a clear example that a data source can be human-friendly but not necessarily machine friendly 
> > {: .output}
> {: .solution}
{: .challenge}

If you want to learn more about the Rich Results Test, you can find it here: [support.google.com/webmasters/](https://support.google.com/webmasters/answer/7445569). 

The FAIR principles rely in the idea of structured data following [Semantic Web](https://en.wikipedia.org/wiki/Semantic_Web) guidelines and formats. All search engines (e.g. Google) and data aggregators (e.g. Elsevier)work with the same standards making it easier to discover datasets. They can understand structured data in web pages about datasets using either [schema.org](https://schema.org/Dataset), Dataset markup or equivalent structures represented in W3C's [Data Catalog Vocabulary (DCAT)](https://www.w3.org/TR/vocab-dcat/) format. 

When you have a project website, or project folder accessible to third parties, you must include the Rich Metadata format in the root folder for the data source to be discoverable and therefore **Reusable**

For example:

    <html>
    <head>
        <title>This Dataset is a FAIR example</title>
        <script type="application/ld+json">
        {
        "@context":"https://schema.org/",
        "@type":"Dataset",
        "name":"Dummmy Data",
        "description":"This is an example for the Bootcamp",
        "url":"https://example.com",
        "identifier": ["https://doi.org/XXXXXX",
                        "https://identifiers.org/XXXX"],
        "keywords":[
            "DUMMY DATA",
            "EXAMPLE FORMAT",
        ],
        "license" : "https://creativecommons.org/publicdomain/zero/1.0/",
        "isAccessibleForFree" : true,
        "funder":{
            "@type": "Organization",
            "sameAs": "https://example.com",
            "name": "NATIONAL FUNDING"
            }
        }
        </script>
    </head>
    <body>
    </body>
    </html>

> ## Exercise - Level Easy 🌶
>
> 1. Visit the dataset you uploaded in the [Data Archiving](https://maastrichtu-library.github.io/qualitative-FAIR-data/05-data-archiving/index.html) episode
> 2. Download the Rich Metadata file (JSON-LD) format  
> **Question:** What similarities do you find with the above example?
> {: .source}
>
> > ## Solution
> >
> > The format is JSON-LD: type="application/ld+json"  
> > The vocabulary is Schema.Org: "@context":"https://schema.org/"  
> > The type is a Dataset: "@type":"Dataset"  
> > {: .output}
> {: .solution}
{: .challenge}


> ## Discussion  
> Secondary use of Qualitative Data?  
>
> The UK Data Service provides an overview on **[Approaches to reusing qualitative data](https://ukdataservice.ac.uk/learning-hub/qualitative-data/reusing-qualitative-data/approaches-to-reusing-qualitative-data/)** such as *Comparative research*, *Reanalysis*, or *Learning and teaching*
> - Discuss with your team how we can extend these categories for secondary use of Qualitative data  
{: .discussion}


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