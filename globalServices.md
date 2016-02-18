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

* [accounts-v1](#accounts-v1)
    * [get-accounts](#get-accounts)
    * [get-accounts-balances](#get-accounts-balances)
    * [patch-accounts_id](#patch-accounts_id)
    * [get-accounts_id](#get-accounts_id)   
    * [get-accounts_id-holds](#get-accounts_id-holds)
    * [post-accounts_id-blocks](#post-accounts_id-blocks)
    * [get-accounts_id-blocks](#get-accounts_id-blocks)
    * [post-accounts_id-participants](#post-accounts_id-participants)
    * [get-accounts_id-participants](#get-accounts_id-participants)
    * [post-accounts_id-checkbooks](#post-accounts_id-checkbooks)
    * [get-accounts_id-checkbooks](#get-accounts_id-checkbooks)
    * [get-accounts_id-transactions](#get-accounts_id-transactions)
    
* [security-v1](#security-v1)
    * [post-token](#post-token)
    * [get-authorize](#get-authorize)
    * [post-reset](#post-reset)
    
* [cards-v1](#cards-v1)
    * [get-cards](#get-cards)
    * [get-cards-balances](#get-cards-balances)
    * [delete-cards_id](#delete-cards_id)
    * [patch-cards_id](#patch-cards_id)
    * [get-cards_id](#get-cards_id)  
    * [get-cards_id-activations](#get-cards_id-activations)   
    * [put-cards_id-activations_id](#put-cards_id-activations_id)    
    * [get-cards_id-blocks](#get-cards_id-blocks)    
    * [put-cards_id-blocks_id](#put-cards_id-blocks_id)
    * [put-cards_id-pin](#put-cards_id-pin)    
    * [get-cards_id-holds](#get-cards_id-holds)
    * [get-cards_id-securityData](#get-cards_id-securityData)
    * [get-cards_id-transactions](#get-cards_id-transactions)

* [observations](#observations)

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
fromDate | Optional | - | Y | - |
moneyFlow | Optional | - | - | - |
order | Optional | - | - | - |
orderBy | Optional | - | - | - |
product | Optional | - | - | - |
relatedContract | Optional | - | - | - |
tag | Optional | - | - | - |
text | Optional | - | - | - |
toAmount | Optional | - | - | - |
toDate | Optional | - | Y | - |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
relatedContract	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.relatedContractId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.product.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.product.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
amount.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
amount.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
postedDate	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
availableDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transactionTimestamp	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
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
financingPayment.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
financingPayment.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.minimumTerm	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.maximumTerm	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.interestRate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.minimumPayment	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizablePayment.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.terms	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
financingPayment.customizedPayment.currentTerm	 | 	Required	 | 	Y	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.interestRate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.repayment	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingPayment.customizedPayment.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
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
notifications	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
notifications.notificationId	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
notifications.product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.product.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
notifications.notificationType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.notificationType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.platform	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.platform.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
notifications.platform.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
notifications.creationDate	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
notifications.modificationDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
notifications.isUnread	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
notifications.description	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
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
notificationsCount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
notificationsUnread	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 

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
products.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
products.product	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.product.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
products.product.name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
products.type	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.type.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
products.type.name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
products.title	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.title.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.title.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
products.description	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
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
originAccount.accountId	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney.amount	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.currency	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
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
wireTransferId	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
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
fromDate	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
originAccount	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
scopeTypeTransfer	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
state	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
toCurrency | 	Optional	 | 	-	 | 	-	 | 	-	 |
toDate	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
transferee	 | 	Optional	 | 	-	 | 	-	 | 	-	 |


* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
wireTransferId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
originAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
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
sentMoney.amount	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.currency	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.isMajor	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
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
date	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
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
originAccount.accountId	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
schedules.destinationAccount.accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
receivedMoney	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
iterations	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
periodicity	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
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
originAccount	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
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
originAccount.number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
originAccount.alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
originAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
destinationAccount.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.bank.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType	 | 	Type of account.	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
destinationAccount.accountType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
sentMoney	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
sentMoney.isMajor	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
receivedMoney	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.amount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
receivedMoney.currency	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transferee.name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
transferee.identityDocument	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
transferee.identityDocument.documentType.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
scopeType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scopeType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
fromDate	 | 	Required	 | 	-	 | Y	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
iterations	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
periodicity	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
periodicity.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
periodicity.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
modificationDate	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
active	 | 	Required	 | 	-	 | 	-	 | 	-	 |

---------------

## accounts-v1 

### get-accounts

Method: __GET__
URI: __/accounts__ 

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
Order	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
Order by	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
accountType.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
accountType.name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
title	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
title.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
title.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
availableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
availableBalance.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
postedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
postedBalance.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-accounts-balances

Method: __GET__
URI: __/accounts/balances__ 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
aggregateAvailableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
aggregateAvailableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
aggregateAvailableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
aggregatePostedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
aggregatePostedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
aggregatePostedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### patch-accounts_id

Method: __PATCH__
URI: __/accounts/{accountId}__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
alias	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-accounts_id

Method: __GET__
URI: __/accounts/{accountId}__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
formats	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
formats.number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
formats.numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
formats.numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
formats.numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
accountType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
accountType.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
accountType.name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
title	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
title.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
title.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	Y	 | 	-	 | 
address	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
address.streetAddress	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
address.city	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
address.region	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
address.country	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
address.zipCode	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
address.alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
openingDate	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContracts	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relatedContractId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
currencies	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.isMajor	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
availableBalance.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
postedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
postedBalance.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
currenciesAvailableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


### get-accounts_id-holds

Method: __GET__
URI: __/accounts/{accountId}/holds__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
holdId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
initialDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
endDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
transactionDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.application	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.application.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.application.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.address	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.address.streetAddress	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.address.city	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.address.region	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.address.country	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.address.zipCode	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.branch.address.alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
origin.user	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
origin.notify	 | 	Required	 | 	-	 | 	-	 | 	-	 | 


### post-accounts_id-blocks

Method: __POST__
URI: __/accounts/{accountId}/blocks__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
block	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
blockId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 |
blockDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-accounts_id-blocks

Method: __GET__
URI: __/accounts/{accountId}/blocks__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
blockId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 |
blockDate	 | 	Required	 | 	-	 | 	-	 | 	-	 |

### post-accounts_id-participants

Method: __POST__
URI: __/accounts/{accountId}/participants__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
participants	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
participants.firstName | 	Required	 | 	-	 | 	-	 | 	-	 | 
participants	.lastName| 	Required	 | 	-	 | 	-	 | 	-	 | 
participants	.relationship | 	Required	 | 	-	 | 	-	 | 	-	 | 
participants.relationship.id | 	Required	 | 	-	 | 	-	 | 	-	 | 
participants.relationship.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

* STATUS 201 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
participantId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-accounts_id-participants

Method: __GET__
URI: __/accounts/{accountId}/participants__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
participantId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
firstName	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
lastName	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relationship	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relationship.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relationship.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### post-accounts_id-checkbooks

Method: __POST__
URI: __/accounts/{accountId}/checkbooks__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
checks	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checks.checkId | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbookId| 	Required	 | 	-	 | 	-	 | 	-	 | 

* STATUS 201 OR 202 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
checks	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checks.checkId | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbookId| 	Required	 | 	-	 | 	-	 | 	-	 |

### get-accounts_id-checkbooks

Method: __GET__
URI: __/accounts/{accountId}/checkbooks__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.checkbookId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.checkbookType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.type.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.type.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.format	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.format.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.format.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.requestDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.deliveryDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.status	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
checkbooks.status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.firstCheckId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
checkbooks.lastCheckId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-accounts_id-transactions

Method: __GET__
URI: __/accounts/{accountId}/transactions__ 

* URI PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
accountId	 | 	Optional	 | 	-	 | 	-	 | 	-	 |

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
financingType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
fromDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
moneyFlow	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
order	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
orderBy	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
tag	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
text	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

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
relatedBill	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedBill.billId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.image	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
activitySector.image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activitySector.image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
tags	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
attachmentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
commentsCount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

---------------
## security-v1

### post-token

Method: __POST__
URI: __/token__ 

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
grant_type	 | 	Required	 | 	-	 | 	-	 | 	-	 |
scope	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
code	 | 	Required	 | 	-	 | 	-	 | 	-	 |
third_party_user_id	 | 	Optional	 | 	-	 | 	-	 | 	-	 |

* REQUEST BODY :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
refresh_token	 | 	Required just for refresh_token	 | 	-	 | 	-	 | 	-	 |
username	 | 	Required just for password	 | 	-	 | 	-	 | 	-	 |
password	 | 	Required just for password	 | 	-	 | 	-	 | 	-	 |

* REQUEST HEADERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
Authorization	 | 	Basic Authorization Header with client credentials using the following format: clientId:clientSecret enconded in Base64	 | 	-	 | 	-	 | 	-	 |

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
access_token	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
expires_in	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
refresh_token	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
refresh_expires_in	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
token_type	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
scope | 	Required	 | 	-	 | 	-	 | 	-	 | 


### get-authorize

Method: __GET__
URI: __/authorize__ 

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
response_type	 | 	Required	 | 	-	 | 	-	 | 	-	 |
client_id	 | 	Required	 | 	-	 | 	-	 | 	-	 |
state	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
scope	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
redirect_uri	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

* REDIRECT RESPONSE :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
code	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
state	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
error	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### post-reset

Method: __POST__
URI: __/reset__ 

__No defined in anypoint__

---------------
## cards-v1

### get-cards

Method: __GET__
URI: __/cards__ 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
number	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType.id	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
cardType.name	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
grantedCredit	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
grantedCredit.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
grantedCredit.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.currentBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.currentBalance.amount	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
availableBalance.currentBalance.currency	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 
availableBalance.postedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.postedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.postedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.pendingBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.pendingBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.pendingBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.currentBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.currentBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.currentBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.postedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.postedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.postedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.pendingBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.pendingBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.pendingBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-cards-balances

Method: __GET__
URI: __/cards/balances__ 

* STATUS 200 Response fields

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
aggregateAvailableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 |
aggregateAvailableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 |
aggregateAvailableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 |
aggregatePostedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 |
aggregatePostedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 |

### delete-cards_id

Method: __DELETE__
URI: __/cards/{cardId}__ 


* URI PARAMETERS: documentId

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |

* STATUS 202 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId	 | 	Required	 | 	-	 | 	-	 | 	-	 |
number	 | 	Required	 | 	-	 | 	-	 | 	-	 |
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 |

### patch-cards_id

Method: __PATCH__
URI: __/cards/{cardId}__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |

* BODY:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
alias | Required | - | - | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
brandAssociation	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
brandAssociation.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
brandAssociation.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
physicalSupport	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
physicalSupport.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
physicalSupport.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
openingDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
expirationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
holderName	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
code	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.period	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.period.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.period.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContracts	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
creditLimit	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.currentValue	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.currentValue.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.currentValue.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.availableLimit	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.availableLimit.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
creditLimit.availableLimit.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.isMajor	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
postedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
unauthorizedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
unauthorizedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
unauthorizedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesUnauthorizedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesUnauthorizedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesUnauthorizedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-cards_id

Method: __GET__
URI: __/cards/{cardId}__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | N | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
number	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
numberType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
cardType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
brandAssociation	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
brandAssociation.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
brandAssociation.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
physicalSupport	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
physicalSupport.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
physicalSupport.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
bank.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
alias	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
openingDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
expirationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
holderName	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
image.url	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.period	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.period.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
paymentMethod.period.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContracts	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.number	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.product.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType.id	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
relatedContracts.relationType.name	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
availableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.authorised	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.authorised.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.authorised.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.posted	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.posted.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
availableBalance.posted.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.authorised	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.authorised.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.authorised.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.posted	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.posted.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
disposedBalance.posted.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
unauthorizedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
unauthorizedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
unauthorizedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
grantedCredit	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
grantedCredit.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
grantedCredit.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currencies.isMajor	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesAvailableBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesPostedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesUnauthorizedBalance	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesUnauthorizedBalance.amount	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
currenciesUnauthorizedBalance.currency	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
 
### get-cards_id-activations

Method: __GET__
URI: __/cards/{cardId}/activations__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
activationId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
isActive	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
startDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
endDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

### put-cards_id-activations_id

Method: __PUT__
URI: __/cards/{cardId}/activations/{activationId}__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |
activationId | Required | - | - | - |

* BODY:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
limits | Required | - | - | - |
limits.amount | Required | - | - | - |
limits.currency | Required | - | - | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
activationId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
activationDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-cards_id-blocks

Method: __GET__
URI: __/cards/{cardId}/blocks__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
blockId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
blockDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### put-cards_id-blocks_id

Method: __PUT__
URI: __/cards/{cardId}/blocks/{blockId}__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |
blockId | Required | - | - | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
blockId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
blockDate	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### put-cards_id-pin

Method: __PUT__
URI: __/cards/{cardId}/pin__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |

* BODY:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
pin | Required | - | - | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
pin	 | 	Required	 | 	-	 | 	-	 | 	-	 | 

### get-cards_id-holds


Method: __GET__
URI: __/cards/{cardId}/holds__ 

* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |

* STATUS 200 Response fields:

__No defined in anypoint__

### get-cards_id-securityData

Method: __GET__
URI: __/cards/{cardId}/securityData__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | N | - |

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
code	 | 	Required	 | 	-	 | 	Y	 | 	-	 | 

### get-cards_id-transactions

Method: __GET__
URI: __/cards/{cardId}/transactions__ 


* URI PARAMETERS:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
cardId | Required | - | - | - |

* QUERY PARAMETERS :

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
financingType	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
fromAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 |
fromDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
moneyFlow	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
order	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
orderBy	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
tag	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
text	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toAmount	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 
toDate	 | 	Optional	 | 	-	 | 	-	 | 	-	 | 

* STATUS 200 Response fields:

Field | Required | Colombia | Chile | Mexico |
-----------------|-----------------|-----------------|-----------------|-----------------|
transactionId	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
relatedContract.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
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
financingType	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingType.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
financingType.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
status.name	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
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
fraudReport.id	 | 	Required	 | 	-	 | 	-	 | 	-	 | 
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

## observations

###Information not available
cards-holds
cards-pin
cards-limits
cards-cancellation
cards-blocks
cards-activation

cards  
   card.expirationDate ???
   card.creditLimit.availableLimit.amount
"card.creditLimit.availableLimit.currency   "
accounts-transactions

* En __/products__ Chile no sabe que es consumers y links por lo que todos los campos con referencia a los campos relacionados vienen con interrogacion

