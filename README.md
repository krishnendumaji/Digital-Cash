# Digital-Cash

Digital Cash Implementation
Written by Rathna Ramesh 
Submitted for class project, Network security, SJSU
Instructed by Dr. Gokay Saldamli

Language:
Python2.7 (3.x compatible with minor changes)

Dependencies:
BitVector
random
Crypto
socket
hashlib

Protocols implemented:
Blind signature
Secret Spliting
commitment protocol (using keyed hash - hmac)

The BankServer.py, CustomerModule.py and MerchantServer.py modules need to run first. Can be run in different machines by replacing the localhost addresses stored in the code to the IP of the systems they are run in.

The UnusedMO.txt file holds the digital cash singed by the bank to be spent. The amount is displayed before the '-*-*-' string. The topmost MO is sent to the merchant always.

The UsedMO.txt file holds the digital cash already sent out the merchant.(To check double spending detection, place one of the digital cash from this folder as the top element of the UnusedMO.txt, the transaction will not pass. The bank would raise, MO already spent message)