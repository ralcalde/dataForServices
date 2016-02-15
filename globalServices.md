#GLOBAL SERVICES

## Index

* [users-V1](#users-V1)
    * [get-users](#get-users)
    
* [documents-v1](#documents-v1)
    * [delete-documents](#delete-documents)
    * [post-documents](#post-documents)
    * [get-documents](#get-documents)

---------------
## users-V1

### get-users

Method: __GET__
URI: __/users/{userId}__ 


* URI PARAMETERS: userIdrequired

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
userId | Required | - | - | - |


* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
userId | Required | - | - | - |
firstName | Required |-| - | - |
lastName | Required | -| - | - |
lastAccessDate |Required | -| - | - |
birthDate | Required | -| - | - |
email | Required | -| - | - |
phoneNumber | Required | -| - | - |
sex | Required | -| - | - |
identityDocument | Required | -| - | - |
identityDocument.documentType | Required | -| - | - |
identityDocument.documentType.id | | -| - | - |
identityDocument.documentType.name | | -| - | - |
identityDocument.documentNumber | | -| - | - |
isEmployee | Required | -| - | - |
image | Optional | -| - | - |
image.id	 | Optional | -| - | - |
image.name | Optional | -| - | - |
image.url | Optional | -| - | - |

-----------------

## documents-v1

### delete-documents

Method: __DELETE__
URI: __/documents/{documentId}__ 


* URI PARAMETERS: documentId

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
documentId | Required | - | - | - |

* STATUS 200 Response fields


Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
documentId | Required | - | - | - |


### post-documents

Method: __POST__
URI: __/documents/{documentId}__ 


* URI PARAMETERS: documentId

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
documentId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
documentId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
file	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
file.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
file.size	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
file.documentFamily	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
file.creationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
file.path	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
file.fileManager	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
taxonomy	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
taxonomy.type	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
taxonomy.metadata	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
taxonomy.metadata.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
taxonomy.metadata.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
user	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
branch	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
branch.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
branch.bank	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
comments	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


### get-documents

Method: __GET__
URI: __/documents/{documentId}__ 

* URI PARAMETERS: documentId

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
documentId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
file	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

