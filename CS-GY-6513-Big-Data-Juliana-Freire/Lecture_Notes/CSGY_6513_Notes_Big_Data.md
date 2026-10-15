# CS-GY 6513: Big Data
- [Hari Varsha V](mailto:hv2241@nyu.edu)
- Fall 2026

## Abstract
These are notes for NYU’s CS-GY 6513, a graduate class on Big Data, as taught by Juliana Freire in Fall 2026. Topics include . 

**Course description**: 

# October 15, 2026

## Introduction - Dataset Search and Discovery
Tons of data available today and enterprises built around it. We start the class off with data warehouses: pretend you're a large company with different sets of data, warehouse is a way to integrate and organize them into one place. Data lake: centralized storage repository that holds vast amounts of structured, semi-structured, and unstructured data in its original, raw format until it is needed for analysis

Challenges: Organizing the schemas and all the datasets in one place.

Machine Learning has become an integral part of Big Data. Example: Use taxi trip data to predict demand. You can either improve the model itself or invest in the right feature to see improvements (such as weather). What kind of data would you analyze to support your hypothesis? 

Case Study: Reduced the speed limit to 25 (NYC Vision Zero), It dipped but fatalities increased (Their objective is to reduce fatalities). Answer: unrelated; citibike and uber launched, so traffic increased and hence fatalities.

How does Google search engine work? Page Rank. Web Search Engines just index all the data. Pre-search engine era, we had yahoo directories where all the websites were 


## Data Lakes:
1. Create a centeralized index of all structured data in an enterprise
2. Decouple data producers from data consumers
3. Supports data governance and lineage/provenance(GDPR, SOC-2, etc. Need to have a way to delete your data in accordance to GDPR if a user requests )
4. Architecture: structured + unstructured data -> extraction (web pages and such) + parsing -> scheme inference -> unified metadata, sketches, data - unified metadata, sketches, data. Query/Search <-> Applications.
5. They basically just store raw data from various formats and need to be on-demand and dynamic.


## Dataset Search Systems
1. Dataset repo: CKAN (gov), Socrata (Based in Seattle, NYC Open Data)
2. Metadata management: Google Goods, AcrylData, Metaphor
3. Data lakes: Delta Lake, Microsoft, Databricks, AWS, Cloudera

Limitations of querying dataset collections: 
1. Difficult to express information needs using keyword based queries and to assess dataset relevance based on textual snippets
2. Metadata can be necessarily incomplete and can be inconsistent with the data.
3. Data changes overtime so your assumptions may not be valid.

Prof explores more about her lab's research.


## Notes 
What's SOTA in search engine these days?

1. Take a crash course in ML and DBs.
2. Learn SQL and PostgreSQL

















