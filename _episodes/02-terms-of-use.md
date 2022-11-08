---
title: "Data Terms of Use"
teaching: 10
exercises: 15
questions:
- "1 What are Data Terms of Use?"
- "2 What a Data Terms of Use statement must contain?"
- "3 What format should Data Terms of Use be?"
- "4 Are there standard Licenses we can pick up from?"
objectives:
- "The participant will understand what data terms of use are with examples."
- "The participant will be able to create basic data terms of use."
keypoints:
- "The Data Terms of Use statement is the legal basis of the referred data source"
- "A License is the bare minimum requirement for Data Terms of Use."
- "If a standard License does not fit your project then you can use Terms of Use layouts e.g. [Sample Data Usage Agreement](https://dataverse.org/best-practices/sample-dua)"
---

> ## FAIR principles used in Data Terms of Use:  
> **Accessible**   
> > FM-A2 (Metadata Longevity) → [doi.org/10.25504/FAIRsharing.A2W4nz](https://doi.org/10.25504/FAIRsharing.A2W4nz)  
>
> **Reusable**  
> > FM-R1.1  (Accessible Usage License) → [doi.org/10.25504/FAIRsharing.fsB7NK](https://doi.org/10.25504/FAIRsharing.fsB7NK)  
>
{: .checklist}

### 1 What are Data Terms of Use?

> Data Terms of Use is a textual statement that set the rules, terms, conditions, actions, legal considerations and licences that delineate data use.  
{: .objectives}

An example is:
<br>
<img title="terms" src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/02-1.png" alt="Terms of Use">
**The World Bank - Terms of Use for Datasets**   → [LINK TO EXAMPLE](https://www.worldbank.org/en/about/legal/terms-of-use-for-datasets)  

Looking at the example, we can identify general elements in the **Data Terms of Use** statement. For instance, a broad description of the data is referred to, but also under what type of license the user is allowed to reuse. 

Sometimes as part of our research, we use commercial databases. We should be careful always to read the conditions for using it for research purposes 
An example is:  
**Terms of Use - Numbeo.com**   → [LINK TO EXAMPLE](https://www.numbeo.com/common/terms_of_use.jsp)    
We can see that clause 3 of Licensing of content requests work attribution.

<img title="terms2" src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/02-4.png" alt="Terms of Use NUMBEO">

### 2 What a Data Terms of Use statement must contain?

As a general rule is that a **Data Terms of Use** statement must contain at least the following:

|Section| Description|Example|
|---|---|---|
|**Description**| What is this statement about and what Digital Objects referred to |*The following Terms of Use statement is about my happy dataset*|
|**License**|Statement under which conditions a requester is allowed to use the data source|*The happy dataset is of Public Domain*|
|**Work attribution**|Statement requesting citation of the data source used |*Could you please cite my happy dataset?*|
|**Disclaimer**| Any consideration that the requester should be aware of|*The last 100 records of my happy dataset might have selection bias*|

Nevertheless, depending on the use case, the "Data Terms of Use" statement can be extended by adding specific clauses when complex data, multiple databases or sensitive data are involved. After all, the "Data Terms of Use" statement is the legal basis of the referred data source. i.e. in the light of public law, you can make someone liable for not complying with specific clauses of the statement. 

Moreover, sometimes our work is conducted within the context of a greater scientific funded project. Therefore, it is always recommended to check with the Principal Investigator or Project Manager whether the **Data Terms of Use** statement is to be defined or if there is already a **Data Policy** framework.

An example is:  
**Policy for use and oversight of samples and data arising from the Biomedical Resource of the 1958 Birth Cohort (National Child Development Study)**   → [LINK TO EXAMPLE](https://fairsharing.org/FAIRsharing.z09fg9)  
- Link to the original [Data Policy](https://cpb-eu-w2.wpmucdn.com/blogs.bristol.ac.uk/dist/7/314/files/2015/07/POLICY-DOCUMENT-FINAL-Vsn-4.0-DEC-2014.pdf)

This policy framework creates comprehensive guidelines on handling data for that specific study involving children's data. Therefore, the researchers working underneath the project do not have to make new Data Terms of Use.

> ## "Data Terms of Use" statement is the legal basis of the referred data source
>
> In the light of public law, you can make someone liable for not complying with specific clauses of the statement.  
{: .callout}

### 3 What format should Data Terms of Use be?

The **Data Terms of Use** is a plain text statement. This text has the length and depth that the data owner or data manager sees fit. There is no right or wrong when drafting it. Usually is recommended to store this textual statement in a `README` file, using an accessible format, for example, `.txt`, `.md` or `.html` so that any user can read it without needing any additional software.

> ## The Data Terms of Use is a plain text statement written in a machine-friendly format
>
> The "Data Terms of Use" can be drafted using any application (e.g. MS Word). However, it's important to store it in a machine-friendly format such as `.txt` or `.md`
{: .callout}

Any text editor software would do the trick, such as [Notepad++](https://notepad-plus-plus.org/) or [Sublime Text](https://www.sublimetext.com/), but also you can write it using Microsoft Word or Google Docs and save it as `.txt` 

> ## Exercise - Level Medium 🌶🌶
>
> 1. Visit the landing page of the following terms of use [github.com/CityOfPhiladelphia/terms-of-use/blob/master/LICENSE.md](https://github.com/CityOfPhiladelphia/terms-of-use/blob/master/LICENSE.md)   
> 2. Can you tell what type of data it is about?   
> 3. Can you tell in what format the terms of use are written?    
> 4. What platform are they using to put it?     
> {: .source}
>
> > ## Solution
> >
> > - Refers to the public code on which the large city of Philadelphia government is based (https://www.phila.gov/)    
> > - The format is Markdown (`.md`)   
> > - They used Github to put the `LICENSE.md` file, which is the Data Terms of Use. 
> > {: .output}
> {: .solution}
{: .challenge}

The **Data Terms of Use** needs to be in the same root folder as the data source. When it comes to a database - like the World Bank example - it should be findable on the project's website. Moreover, if there is no official project website, you should include it in `.md` format in a Github repository like the following example: → [LINK TO EXAMPLE](https://github.com/MaastrichtU-IDS/clean-technologies-nlp/blob/master/data/README.md)  

<img title="terms3" src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/02-2.png" alt="Terms of Use folder">

In [Episode 4 (Data Archiving)](https://maastrichtu-library.github.io/circular-research-data-bootcamp/06-rich-metadata/index.html), we will explore that some data repositories such as [DataverseNL](dataverse.nl/) allow you to create a Data Terms of Use statement directly on the platform when you create a data project.   
By default, you get a waiver License [CC0 “No Rights Reserved”](https://creativecommons.org/share-your-work/public-domain/cc0/). Putting a database or dataset in the public domain under CC0 is a way to remove any legal doubt about whether researchers can use the data in their projects. Although CC0 doesn’t legally require data users to cite the source, it does not affect the ethical norms for attribution in scientific and research communities. Moreover, you can change this waiver to a tailored Terms of Use you have created for your data.

<img title="terms4" src="https://maastrichtuniversity-ids-open.s3.eu-central-1.amazonaws.com/images/02-3.png" alt="License is part of the Terms of Use">
<br>


> ## Exercise - Level Easy 🌶
>
> Is it possible to edit the Terms of Use in DataverseNL?
>
> Go to [DataverseNL/](https://dataverse.nl/) to the FAQ section t find out.
> {: .source}
>
> > ## Solution
> >
> > Yes, it is possible. However, you can't choose it at the beginning. After creating a dataset, go to the ‘Terms’ tab on your dataset page and click ‘Edit Terms requirements’. Next, select the radio button ‘No, do not apply CC0 public domain dedication’, and fill in the text fields with your terms and conditions.
> >
> > {: .output}
> {: .solution}
{: .challenge}

> Dataverse also provides **Sample Data Usage Agreement** →  [LINK](https://dataverse.org/best-practices/sample-dua)
{: .prereq}

### 4 Are there standard Licenses we can pick up from?

Yes, there are two general License frameworks that can work for data.  

> - [Creative Commons (CC)](https://creativecommons.org/about/cclicenses/)  
> - [Open Data Commons (ODC)](https://opendatacommons.org/licenses/index.html)  
{: .prereq}

[Creative Commons (CC)](https://creativecommons.org/about/cclicenses/) provides several licenses that can be used with a wide variety of creations that might otherwise fall under copyright restrictions, including music, art, books and photographs. Although not tailored for data, CC licenses can be used as data licenses because they are easy to understand. Its website includes a summary page [HERE](https://creativecommons.org/about/cclicenses/) outlining all the available licenses, explained with simple visual symbols.

|Permission Mark|What can I do with the data?|
|---|---|
|BY|Creator must be credited|
|SA|Derivatives or redistributions must have identical license|
|NC|Only non-commercial uses are allowed|
|ND|No derivatives are allowed|

[Open Data Commons (ODC)](https://opendatacommons.org/licenses/index.html) provides three licenses that can be explicitly applied to data. The web pages of each of these licenses include human-readable summaries, with the ramifications of the legalese explained in a concise format.

---

> ## Exercise - Level Easy 🌶
>
> Pick up a License at [creativecommons.org](https://creativecommons.org/share-your-work/) with the following conditions:  
> - Others cannot make changes to the work since it's simulation data
> - If someone wants to use the simulation data for a startup, they can 
> **Question:** What type of license is it?
> {: .source}
>
> > ## Solution
> >
> > Attribution-NoDerivatives 4.0 International
> >
> > {: .output}
> {: .solution}
{: .challenge}


> ## Discussion  
> Real case:  
The Swedish DPA (Integritetsskyddsmyndigheten) fined Umeå University SEK 550,000 (EUR 54,000) as a result of its failure to apply appropriate technical and organizational measures to protect data. As part of a research project on male rape, the university had stored several police reports on such related incidents in the cloud of a U.S. service provider. The reports contained the names, ID numbers and contact details of the data subjects, as well as information about their health and sex lives, alongside information about the suspected crime [LINK TO CASE](https://www.enforcementtracker.com/ETid-482)
> 
> Discuss with your team how using legal instruments (in the context of the research) such as data terms of use or data protection impact assessment can be helpful in such situations.
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