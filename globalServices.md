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
    * [delete-deviceId](#delete-deviceId)
    * [patch-deviceId](#patch-deviceId)
    * [put-deviceId](#put-deviceId)
    * [get-deviceId](#get-deviceId)

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

### delete-deviceId

Method: __DELETE__
URI: __/devices/{deviceId}__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
deviceId | Required | - | - | - |

### patch-deviceId

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

### put-deviceId

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

### get-deviceId

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

