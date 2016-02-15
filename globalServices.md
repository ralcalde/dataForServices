#GLOBAL SERVICES

## Index

* [users-V1](#users-V1)
    * [/users/{userId}-GET](#/users/{userId}-GET))
    
* [documents-v1](#documents-v1)
    * [/documents/{documentId}-DELETE](#DELETE-documents)
    * [/documents/{documentId}-POST](#/documents/{documentId}-POST)
    * [/documents/{documentId}-GET](#/documents/{documentId}-GET)

---------------
## users-V1

### /users/{userId}-GET

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

### DELETE-documents

* URI PARAMETERS: documentId

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
documentId | Required | - | - | - |

* STATUS 200 Response fields


Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
documentId | Required | - | - | - |

### /documents/{documentId}-POST

### /documents/{documentId}-GET


