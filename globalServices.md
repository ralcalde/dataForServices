#GLOBAL SERVICES

## Index

* [users-V1](#users-V1)
    * [get-users](#get-users)
    
* [documents-v1](#documents-v1)
    * [delete-documents](#delete-documents)
    * [post-documents](#post-documents)
    * [get-documents](#get-documents)

* [transactions-v1](#transactions-v1)
    * [get-transactions](#get-transactions)
    * [get-transactions-balances](#get-transactions-balances)
    * [get-transactions-tags](#get-transactions-tags)
    * [get-transactions-id](#get-transactions-id)
    * [get-transactions-comments](#get-transactions-comments)
    * [get-transactions-attachments](#get-transactions-attachments)
    * [get-transactions-fees](#get-transactions-fees)
    * [get-transactions-commerce](#get-transactions-commerce)

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

---------------

## transactions-v1

### get-transactions

Method: __GET__
URI: __/transactions__ 

* QUERY PARAMETERS: documentId

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
financingType | Optional | - | - | - |
fromAmount | Optional | - | - | - |
fromDate | Optional | - | - | - |
moneyFlow | Optional | - | - | - |
order | Optional | - | - | - |
orderBy | Optional | - | - | - |
product | Optional | - | - | - |
relatedContract | Optional | - | - | - |
tag | Optional | - | - | - |
text | Optional | - | - | - |
toAmount | Optional | - | - | - |
toDate | Optional | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.relatedContractId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.product.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.product.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transactionTimestamp	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
concept	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
concept.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
concept.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
concept.image	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
concept.image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
concept.image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
concept.image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
moneyFlow	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
moneyFlow.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
moneyFlow.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkNumber	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
availableBalance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
availableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
postedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.minimumTerm	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.maximumTerm	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.interestRate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.minimumPayment	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.terms	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.currentTerm	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.interestRate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.repayment	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fraudReport	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fraudReport.fraudReportId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fraudReport.status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fraudReport.status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fraudReport.status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fraudReport.reason	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fraudReport.comments	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedBill	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedBill.billId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.image	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
activitySector.image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
points	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
points.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
points.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
points.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.promotionType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.promotionType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.promotionType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.discount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.discount.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.discount.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.originAmount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.originAmount.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
appliedPromotions.originAmount.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
tags	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachmentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
commentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 



### get-transactions-balances

### get-transactions-tags

### get-transactions-id

### get-transactions-comments

### get-transactions-attachments

### get-transactions-fees

### get-transactions-commerce


