# Creating Blob Storage

## Objective
Create a Blob storage to store some data (csv file).

## Steps I took
1. Entered my Personal Project's resource group -> Resources.
2. Located Storage Account on Marketplace and created a storage account. 
3. Set Primary service to 'Azure Blob Storage or Azure Data Lake Storage'. 
4. Altered redundancy to LRS, as my data holds no great importance at the moment. 
5. Left remaining settings as default (not suggested for live projects/solutions).
6. Added my workload tag.
7. Reviewed and created.
8. Within the storage account created a container, deafult private access
9. Uploaded a csv file to the blob. Was now able to view and edit it.
10. Deleted the storage container.


## Screenshot

## What I learned
- To first create a Blob Storage, you'll need a storage account.
- Storage account names must be unique and are not allowed hyphens or underscores or captial letters. I decided to follow a similar format as resource groups, just without the hyphens: {prefix}{workload}{environment}{region}.
- Geo-redundant storage is for backup scenarios (across regions)
- Zone-redundant storage is for high availability scenarious (across datacenters)
- For networking it is a big risk to leave public access on. A secure solution would be private, with moderated access.
- Storage accounts are charged for the amount of data that is stored. By default a tiny cost will be incurred for metdata etc (yet to see this in action will come back and test tomorrow. - no charges incurred)
- By setting the csv file as private, I will not be able to access/view the file via URL.


## Gotchas
Tried to find blob storage on the marketplace, but it was actually under storage account.
Storage account name must be between 3-24 characters.
Containers are part of Blob storage, Blobs are the files themsevles. Blob storage often means the whole stack (Storage account + container + Blobs)
