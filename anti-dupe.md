# Anti-Duplication 
In order to prevent a card from being read multiple times, we must process them in some way when they are recieved for the first time. A simple way to do this from a physical perspective would be to tear or fold a card when recieved. If this is not permited however, then we must use one of our 4 ASCII characters to denote this information. 

## Physical Anti-Duplication
If we can make physical alterations to notecards, then a reciever of a notecard can dog-ear the card to denote that the message was successfully recieved, without destroying the card. This is like the equivolant of having a read receipt on a text message or email, which prevents the user from accidently processing information twice, but keeps the information for future reference. This will be needed when multiple cards are needed to convey one message.

## ASCII Anti-Duplication 
Similarly, a single ASCII character could be used to denote read vs unread messages. This value could always start as 0, and be updated to 1 when the message is recieved.
