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

* [devices-v1](#devices-v1)
    * [get-devices](#get-devices)
    * [delete-deviceid](#delete-deviceid)
    * [patch-deviceid](#patch-deviceid)
    * [put-deviceid](#put-deviceid)
    * [get-deviceid](#get-deviceid)

* [notifications-v1](#notifications-v1)
    * [put-notifications](#put-notifications)
    * [get-notifications](#get-notifications)
    * [post-notifications-configuration](#post-notifications-configuration)
    * [get-notifications-configuration](#get-notifications-configuration)   
    * [get-notifications-count](#get-notifications-count)

* [products-v1](#products-v1)
    * [get-products](#get-products)

* [wire_transfers-v1](#wire_transfers-v1)
    * [post-wire_transfers](#post-wire_transfers)
    * [get-wire_transfers](#get-wire_transfers)
    * [delete-wire_transfers_id](#delete-wire_transfers_id)
    * [get-wire_transfers_id](#get-wire_transfers_id)    
    * [get-wire_transfers_id-limits](#get-wire_transfers_id-limits)
    * [delete-wire_transfers-destination_accounts](#delete-wire_transfers-destination_accounts)
    * [post-wire_transfers-destination_accounts](#post-wire_transfers-destination_accounts)
    * [get-wire_transfers-destination_accounts](#get-wire_transfers-destination_accounts)
    * [delete-wire_transfers-schedules](#delete-wire_transfers-schedules)
    * [put-wire_transfers-schedules](#put-wire_transfers-schedules)
    * [post-wire_transfers-schedules](#post-wire_transfers-schedules)
    * [get-wire_transfers-schedules](#get-wire_transfers-schedules)


## wireTransfers-v1

### post-wireTransfers

### get-wireTransfers

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


* BODY :

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

* URI PARAMETERS:

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

* QUERY PARAMETERS:

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

Method: __GET__
URI: __/transactions/balances__ 

* QUERY PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
fromDate | Optional | - | - | - |
toDate | Optional | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
differentialBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
differentialBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
differentialBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
purchasingVariation	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
purchasingVariation.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
purchasingVariation.unit	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.month	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.year	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.incomes	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.incomes.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.incomes.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.expenses	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.expenses.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.expenses.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.differentialBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.differentialBalance.amount	 | 	Optional???	 | 	-	 | 	-	 | 	-	 | 
balanceSheet.differentialBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


### get-transactions-tags

Method: __GET__
URI: __/transactions/tags__ 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
tagsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 |
tags	 | 	Required	 | 	-	 | 	-	 | 	-	 |

### get-transactions-id

Method: __GET__
URI: __/transactions/{transactionId}__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
product.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
product.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAmount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAmount.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAmount.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
type	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
type.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
type.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
moneyFlow	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
moneyFlow.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
moneyFlow.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.isMajor	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
availableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
postedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
tags	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachmentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
commentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


### get-transactions-comments

Method: __GET__
URI: __/transactions/{transactionId}/comments__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
commentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
comments	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
comments.commentId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
comments.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
comments.lastUpdate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
comments.private	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-transactions-attachments

Method: __GET__
URI: __/transactions/{transactionId}/attachments__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
attachmentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.attachmentId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.filename	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.filedata	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.mimetype	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.size	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.lastUpdate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachments.private	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-transactions-fees

Method: __GET__
URI: __/transactions/{transactionId}/fees__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
feesCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fees	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fees.feeId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fees.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fees.balance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fees.balance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fees.balance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


### get-transactions-commerce

Method: __GET__
URI: __/transactions/{transactionId}/commerce__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
commerceId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
geolocalization	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
geolocalization.latitude	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
geolocalization.longitude	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

---------------

## devices-v1

### get-devices

Method: __GET__
URI: __/devices__ 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId	 | 	Required	 | 	-	 | 	-	 | 	-	 |
token	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

### delete-deviceid

Method: __DELETE__
URI: __/devices/{deviceId}__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId | Required | - | - | - |

### patch-deviceid

Method: __PATCH__
URI: __/devices/{deviceId}__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId | Required | - | - | - |

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
alias | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId	 | 	Required	 | 	-	 | 	-	 | 	-	 |
token	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

### put-deviceid

Method: __PUT__
URI: __/devices/{deviceId}__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId | Required | - | - | - |

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
token | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId	 | 	Required	 | 	-	 | 	-	 | 	-	 |

### get-deviceid

Method: __GET__
URI: __/devices/{deviceId}__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId	 | 	Required	 | 	-	 | 	-	 | 	-	 |
token	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 


---------------
## notifications-v1

### put-notifications

Method: __PUT__
URI: __/notifications__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
notifications | Required | - | - | - |
notifications.notificationId | Required | - | - | - |
notifications.isUnread | Required | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
notificationId	 | 	Required	 | 	-	 | 	-	 | 	-	 |


### get-notifications

Method: __GET__
URI: __/notifications__ 

* QUERY PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
platform | Optional | - | - | - |
priority | Optional | - | - | - |
product | Optional | - | - | - |
type | Optional | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
notificationsNew	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notificationsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.platform	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.platform.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.platform.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.creationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.modificationDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.isUnread	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.description	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.parameters	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.parameters.key	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.parameters.value	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.parameters.parameter	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.parameters.parameter.key	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.parameters.parameter.value	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.priority	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.priority.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.priority.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

### post-notifications-configuration

Method: __POST__
URI: __/notifications/configuration__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
notifications | Required | - | - | - |
notifications.product | Required | - | - | - |
notifications.activate | Required | - | - | - |
notifications.platform | Optional | - | - | - |
notifications.platform.id | Optional | - | - | - |
notifications.platform.name | Optional | - | - | - |
notifications.priority | Optional | - | - | - |
notifications.conditions | Optional | - | - | - |
notifications.conditions.id | Optional | - | - | - |
notifications.conditions.value | Optional | - | - | - |
notifications.conditions.currency | Optional | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
notifications	 | 	Required	 | 	-	 | 	-	 | 	-	 |
notifications.notificationId	 | 	Required	 | 	-	 | 	-	 | 	-	 |

### get-notifications-configuration


Method: __GET__
URI: __/notifications/configuration__ 

* QUERY PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
platform | Optional | - | - | - |
product | Optional | - | - | - |
type | Optional | - | - | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
notificationsConfigurationId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
configurable	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
conditionable	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
platform	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
platform.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
platform.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
platform.active	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
priority	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
priority.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
priority.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
conditions	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
conditions.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
conditions.condition	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
conditions.value	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
conditions.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 


### get-notifications-count


Method: __GET__
URI: __/notifications/count__ 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
notificationsNew	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notificationsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notificationsUnread	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

---------------

## products-v1

### get-products

Method: __GET__
URI: __/products__

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
consumers	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
consumers.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
consumers.productsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.product.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.product.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.type	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.type.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.type.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.title	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.title.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.title.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.description	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.consumers	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.consumers.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.consumers.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

---------------

## wire_transfers-v1

### post-wire_transfers

Method: __POST__
URI: __/wireTransfers__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
originAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.isNegotiated	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
charges	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
urgentTransfer	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.contactInformation	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.platform	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
isSimulated	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


* STATUS 201 or 202 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
wireTransferId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
approxReceptionTransferDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fees	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.isNegotiated	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 


### get-wire_transfers


Method: __GET__
URI: __/wireTransfers__ 

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
destinationAccountNumber	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
destinationAccountNumberFormat	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromCurrency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
originAccount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeTypeTransfer	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
state	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
toCurrency | 	Optional	 | 	-	 | 	-	 | 	-	 |
toDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Optional	 | 	-	 | 	-	 | 	-	 |


* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
wireTransferId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.isMajor	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.isNegotiated	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
charges	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
charges.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
charges.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
date	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
urgentTransfer	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.value	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.period	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.period.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.period.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
 

### delete-wire_transfers_id

Method: __DELETE__
URI: __/wireTransfers/{wireTransferId}__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
wireTransferId	 | 	required	 | 	-	 | 	-	 | 	-	 |

### get-wire_transfers_id

Method: __GET__
URI: __/wireTransfers/{wireTransferId}__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
wireTransferId	 | 	required	 | 	-	 | 	-	 | 	-	 |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
wireTransferId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.isMajor	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.balance.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fees.isNegotiated	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
charges	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
charges.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
charges.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
date	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
urgentTransfer	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.value	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.period	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.period.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
cancellationInterval.period.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 


### get-wire_transfers_id-limits

Method: __GET__
URI: __/wireTransfers/{wireTransferId}/limits__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
wireTransferId	 | 	required	 | 	-	 | 	-	 | 	-	 |

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
name	 | 	optional	 | 	-	 | 	-	 | 	-	 |


* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
limitId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount.value	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### delete-wire_transfers-destination_accounts

Method: __DELETE__
URI: __/wireTransfers/destinationAccounts__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
originAccountId	 | 	required	 | 	-	 | 	-	 | 	-	 |

### post-wire_transfers-destination_accounts

Method: __POST__
URI: __/wireTransfers/destinationAccounts__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
isFavourite	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 |


* STATUS 201 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
destinationAccountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-wire_transfers-destination_accounts

Method: __GET__
URI: __/wireTransfers/destinationAccounts__ 

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
number	 | 	optional	 | 	-	 | 	-	 | 	-	 |


* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
originAccountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### delete-wire_transfers-schedules

Method: __DELETE__
URI: __/wireTransfers/schedules__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
scheduleId	 | 	required	 | 	-	 | 	-	 | 	-	 |

### put-wire_transfers-schedules

Method: __PUT__
URI: __/wireTransfers/schedules__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
scheduleId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney.isMajor	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fromDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
iterations	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
periodicity	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
active	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
scheduleId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### post-wire_transfers-schedules

Method: __POST__
URI: __/wireTransfers/schedules__ 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
originAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
schedules.destinationAccount.accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
iterations	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
periodicity	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
active	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


* STATUS 201 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
scheduleId	 | 	Required	 | 	-	 | 	-	 | 	-	 |
 

### get-wire_transfers-schedules

Method: __GET__
URI: __/wireTransfers/schedules__ 

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
active	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
concept	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccountNumber	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccountNumberFormat	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromCurrency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
originAccount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeTypeTransfer	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toCurrency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
scheduleId	 | 	Required	 | 	-	 | 	-	 | 	-	 |
originAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType	 | 	Type of account.	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney.isMajor	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fromDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
iterations	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
periodicity	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
periodicity.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
periodicity.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
modificationDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
active	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
 
