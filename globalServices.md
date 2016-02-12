#GLOBAL SERVICES

## Index

* [users-V1](#users-V1)
	* [/users/{userId}](#/users/{userId})
		* [/users/{userId}-GET](#/users/{userId}-GET)	
	* [Example](#example)

## users-V1

### /users/{userId}

#### /users/{userId}-GET

* URI PARAMETERS: userIdrequired, string
* STATUS 200 Response fields

Field | Type	| Required | Description | Chile | Mexico
-----------------|-----------------|-----------------|-----------------|-----------------|-----------------|
userId | String | Required | User identifier | - | - |
firstName | String | Required | User name.| - | - |
lastName | 	String | Required | User last name.| - | - |
lastAccessDate | Date | Required | User last access date (ISO-8601 format).| - | - |
birthDate | Date	 | Required | User birthdate (ISO-8601 format).| - | - |
email | String | Required | Mail user validated by the bank to operate.| - | - |
phoneNumber | String	 | Required | Phone user validated by the bank to operate.| - | - |
sex | String | 	Required | 	User gender.| - | - |
identityDocument | Object | Required | Object where the identity document information is stored.| - | - |
identityDocument.documentType | Object | Required | Object where the type identity document is stored.| - | - |
identityDocument.documentType.id | String | | Identifier associated to type identity document| - | - |
identityDocument.documentType.name | String |  | A description of the type identity document.| - | - |
identityDocument.documentNumber | String |  | Number of identity document| - | - |
isEmployee | Boolean | Required | Flag that identify if the user is employee.| - | - |
image | Object | Optional | Object where the image information of the user is stored.| - | - |
image.id	String | Optional | User image identifier.| - | - |
image.name | String | Optional | A description of the image.| - | - |
image.url | String | Optional | URL to the user image.| - | - |



