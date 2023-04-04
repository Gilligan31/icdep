# Extension

## Assumptions
Unfortunately, some assumptions need to be made in some of these rather complex extenstions to ICDEP. I cannot see any reasonable system where this would function without some breaking of the rules established in class. 

* Some nodes will need mobility. We cannot rely on extremely long arms or wait times to get an index card a mile across campus
* We need more information than a person on campus's name. Even if you knew the person, their wherabouts would (hopefully) not be known by you at all times. We will assume everyone on campus is an active student with a UW student ID which holds their course schedule.
* Any node can use this student ID and MyUW to lookup the recipients class locations and times. 

## Send to any Individual on Campus 
To add this functionality, we will use student ID in the FROM and TO fields of the index card (top right and bottom right respectively). From here we could hypothetically map the student ID to their frequented classrooms - allowing nodes to either pass off the card or deliver it themselves. For this reason we may choose to add another field to the bottom-middle with the priority of the message. Each priority (low, med, high) would have a different threshold for how far out of their way a node should go to acomplish the task. For example, low priority would be completed if the destination was within 15 minutes; 30 minutes for medium, and an hour for high. Otherwise, the node passes the card to the next node. After 10 passes the request would be dropped. Unfortunately, this system has serious limmitations for long messages, as the odds that one card is not delivered is highly probable.

## Specify Data Type
This functionality is rather easy to add, as we can just add another field with the data type (ASCII, Unicode, Binary)

## Node Record 
As long as each node can write, this is another simple functionality to add. The back of the notecard could be used to add a comma separated list of all nodes that acknowledge recieving a note card. If nodes are unable to add data to the card, this would be extremely challenging, as message sender or reciever would have to actively observe the path of their notecard, and then sharing this information would be rather complex.
