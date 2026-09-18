# Open Science

While open science (including research data management, RDM, workflows) has been propagated for several decades, it has only become a central part of ongoing research initiatives in recent years.
I am convinced that well-implemented RDM workflows improve the organization, evaluation, and dissemination of scientific results.
Automation removes the burden of repetitive tasks and creates more room for scientific thinking.
Funding agencies are very aware of the advantages of such implementations; therefore, providing clear information on data handling has become a key criterion for the acceptance of research proposals.

In my opinion, some key challenges are:

* developing systems that remove, rather than create, administrative burdens (which are often associated with this topic),
* convincing stakeholders of all experience levels, from students to project PIs, of the necessity, and
* simplifying access to the vast number of generic and domain-specific tools

## Teaching

An important aspect is the inclusion of open science thinking in the curriculum as well as the development of strategies to get students and teachers alike involved in this topic. An overview of related activities is available in the [Current RDM-related projects](teaching.md#current-rdm-related-projects) subsection on the teaching page.

## Laboratory

In the institute I create incentives for the use of programmatic approaches (mainly Python) to evaluate data.
We foremost address problems that usually consume a lot of time (the boring stuff) or could yield additional scientific insights that cannot be gained from commonly used spreadsheet-based programs (Excel, Origin, ...).

A central part is the storage of data with metadata during data acquisition, which we address with [autotag-metadata](https://github.com/echemdb/autotag-metadata). Data acquired in this way can be reused in automated workflows and in the creation of local databases.

## echemdb

Specific research topics require domain-specific approaches. For the field of electrochemistry, we created the echemdb open-science initiative.
It provides tools and data formats to make electrochemical data FAIR (findable, accessible, interoperable, and reusable). See the dedicated [echemdb page](echemdb.md), the [echemdb website](https://www.echemdb.org), and the [GitHub organization](https://github.com/echemdb/) for details.

## Electronic Lab Notebook (ELN)

Electronic Lab Notebooks play a central part in organizing research data.
So far we mostly explored the use of [MediaWiki](https://www.mediawiki.org/) as an ELN, which is ideal for documentation purposes.
Aside from that, we explore the integration of our local data management tools, specifically [unitpackage](https://echemdb.github.io/unitpackage/) and [autotag-metadata](https://github.com/echemdb/autotag-metadata), in workflows that generate ELN entries automatically to remove the manual task of clicking through the ELN interface.

## Software Contributions

Further software contributions can be found in my [GitHub profile](https://github.com/DunklesArchipel) and the [echemdb organization](https://github.com/echemdb).
