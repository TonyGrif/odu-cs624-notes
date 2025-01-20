# ETL
Extract, transform, and load (ETL) is the process used by data engineers to parse raw data into usable, trusted, structured data.
## Process
* **Extract**: The process of acquiring heterogeneous data from differing data sources
	* **Partial Extraction**: Source system notifies on record change
	* **Full Extraction**: Source system cannot identify when a change has occurred; data must be extracted out and compared to the last copy of the record
* **Transform**: Data is transformed into a format that can be used by applications; this often involves mapping to a specific schema; quality and integrity of data is ensured in this step
* **Load**: Converted data is uploaded to a target database
## Pipeline
An ETL pipeline is a set of tools and processes to automate the [[#Process | ETL process]].
## Resources
* [ETL](https://www.databricks.com/discover/etl)