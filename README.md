# archivesspace-data-collection :sparkles:

**secrets.py**

To use these ArchivesSpace scripts, you must create a secrets.py file in the same directory that contains the following text:

  baseURL='ArchivesSpace API URL'
	user='user name'
	password='password'

*** 

**getEntitiesNotPublished.py**(/getEntitiesNotPublished.py)

This script pulls unpublished entities (where Publish = False) from ArchivesSpace and lists them in a CSV file.

Using the argparse module, the user enters in the terminal either "people," "corporate_entities," or "families" to search for unpublished entities under those categories.The CSV also prints several properties of the unpublished agent, which can be adjusted in the script based on information needs.

|uri                 |publish |name                  |create_time          |rules |created_by |
|--------------------|--------|----------------------|---------------------|------|-----------|
|/agents/families/24 |False   |Smith Family (Alaska) | 2017-03-09T13:29:00z|dacs  |jmarch     |
