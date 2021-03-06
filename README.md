# SciBase GraphDB API
___
> This API is currently still under **active development**. Do not implement/deploy builds of the API without understanding the risks involved.

### CRUD Methods for SciBase Backend Operations
SciBase GraphDB API is a python API library maintained for access to the *SciBase GraphDB*. The different categories of exposed methods are as follows:-
  - *Geophysical* Nodes CRUD Methods
  - *Entity* Nodes CRUD Methods
  - *Member* Nodes CRUD Methods
  - *Computed Relationships* CRUD Methods

For more information, contact 
  - [Snehanshu Saha]
  - [Sandesh Sanjay Gade]

### Version
0.0.1

### Documentation

+ Proposed Methods:-
  - **Geophysical Nodes CRUD Methods**
    1. create_country_nodes([country_names])
    2. create_continent_nodes([continent_names])
    3. attach_countries_to_continent([country_name, continent_name])
    4. get_countries()
    5. get_countries_by_continent(continent_name)
    6. get_continents()
    7. delete_country_nodes([country_names])
    8. delete_continent_nodes([continent_names])
  - **Entity Nodes CRUD Methods**
    1. create_journal_nodes([TUPLE(journal_name, journal_publisher, journal_domain, journal_ISSN, journal_country)])
    2. create_article_nodes([TUPLE(article_title, article_DOI, article_citation_count, article_self_citation_count, article_downloads_count, article_source_cites_count, article_month, article_year, [author_names])])
    3. attach_articles_to_journals([TUPLE([article_DOIs], journal_name]))
    4. get_journals()
    5. get_journals_by_domain(domain)
    6. get_journals_by_country(country_name)
    7. get_journals_by_continent(continent_name)
    8. get_journals_by_publisher(publisher_name)
    9. get_articles_by_primary_author(primary_author_name)
    10. get_articles_by_domain(domain)
    11. get_articles_by_country(country_name)
    12. get_articles_by_continent(continent_name)
    13.	get_articles_by_journal(journal_name)
	14.	delete_journal_nodes([TUPLE(journal_name, journal_ISSN)])
	15.	delete_article_nodes([TUPLE(article_title, article_DOI)])
	16.	update_journal_nodes([TUPLE(TUPLE(journal_name, journal_ISSN), TUPLE(journal_new_name, journal_new_publisher, journal_new_domain, journal_new_ISSN, journal_new_country))])
	17.	update_article_nodes([TUPLE(TUPLE(article_title, article_DOI, article_primary_author), TUPLE(article_new_title, article_new_DOI, article_new_citation_count, article_new_self_citation_count, article_new_downloads_count, article_new_source_cites_count, article_new_month, article_new_year, [article_new_author_names]))])
	18.	create_domain([domain_names])
	19.	attach_subdomain_to_domain([TUPLE(subdomain_name, domain_name)]) 
  - **Member Nodes CRUD Methods**
    1.	create_author_nodes([TUPLE(author_first_name, author_last_name, author_email, author_affiliation, author_origin_country, author_resident_country)])
	2.	get_authors()
	3.	get_authors_by_affiliation(author_affiliation)
	4.	get_authors_by_origin_country(author_origin_country)
	5.	get_authors_by_resident_country(author_resident_country)
	6.	get_authors_by_domain(domain)
	7.	update_author_nodes([TUPLE(TUPLE(author_first_name, author_last_name, author_previous_affiliation), TUPLE(author_new_first_name, author_new_last_name, author_new_email, author_new_affiliation, author_new_origin_country, author_new_resident_country)])
	8.	delete_author_nodes([TUPLE(author_first_name, author_last_name)])
	9. 	create_publisher_nodes([TUPLE(publisher_name, publisher_base_country)])
	10.	get_publishers()
	11.	get_publishers_by_country(country_name)
	12.	get_publishers_by_domain(domain)
	13.	update_publisher_nodes([TUPLE(TUPLE(publisher_name, publisher_base_country), TUPLE(publisher_new_name, publisher_new_base_country))])
	14.	delete_publisher_nodes([TUPLE(publisher_name, publisher_base_country)])
	15.	create_affiliation_nodes([TUPLE(affiliation_name, affiliation_country)])
	16.	delete_affiliation_nodes([affiliation_name])
	17.	get_affiliations()
	18.	get_affiliations_by_country(country_name)
	19.	get_affiliations_by_domains(domain)
  - **Computed Relationships CRUD Methods**

### Installation

Installing Hug/Falcon

```sh
$ //add hug/falcon installation instructions here
```

```sh
$ add some more code here. Saijal made some changes here!
```

### Plugins


### Development

Want to contribute? Great! Scroll to the top of this document to find contact information about the developers.

### Docker

More details coming soon.

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)
   [snehanshu saha]: <snehanshusaha@pes.edu>
   [sandesh sanjay gade]: <fb.com/cyberbeast>
