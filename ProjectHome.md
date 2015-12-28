# Example #
```
>>> from pypostbank import *
>>> a = getAccount(9999999999, 11111)
>>> a.name
'Girokonto'
>>> a.holder
'PETRA PFIFFIG'
>>> a.bankCode
20010020
>>> a.accountNumber
9999999999L
>>> a.IBAN
'DE31200100209999999999'
>>> a.balance
Decimal("5314.05")
>>> a.outstandingMoney
Decimal("0.00")
>>> record = a.accountingRecords[0]
>>> print "information =", record.information
information = 111111/1000000000/37050198 FINANZKASSE 3991234 STEUERNUMMER 00703434
>>> print "kind =", record.kind
kind = Überweisung
>>> print "intiator = ", record.initiator
intiator =  PETRA PFIFFIG
>>> print "amount =", record.amount
amount = -328.75
>>> print "valueDate =", record.valueDate
valueDate = 2007-05-20
>>> print "date =", record.date
date = 2007-05-20
>>> print "balance =", record.balance
balance = 5314.05
>>> print "recipient =", record.recipient
recipient = Finanzkasse Köln-Süd
```

