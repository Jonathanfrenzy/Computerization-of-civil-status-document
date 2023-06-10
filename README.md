## Computerization-of-civil-status-document(CCSD)
the login credentials are 
username: joseph
password: alpharogue**

## Review of what is a CCSD
CCSD is a system for computerizing civil status documents(like birth certificate or marriage certificate) into government built databases(servers) and archiving of those documents and the various ways in which those documents can be recovered by the citizens.
CCSD also deals with decreasing the level of office work in government offices by pushing simple procedural processes such as certification to the online space.

To archieve this a system with multiple level users was built. The system was built in such a way that only the highest level user has access to the database and can modify the data in the database.
The various users of the system are:
-secretary
-manager
-superadmin

# the secretary
The secretary is the lowest level user of the system.
They principally work only for entering citizen data with a scanned copy of the citizen's document into the database.
They can also print out citizen's document in case if a citizen loses his documents
They also certify soft copy of those documents in the online space.
They have no access to the database 

# the manager
The manager is a mid-level user of the system.
The manager has access to the database but it is only limited to viewing not changing the information of te databse
He supervises the work done by the secretaries by viewing all the records the secretary accounts add into the database
He grants the secretaries account temporal limited access to the database
He grants the secretaries digital stamps to apply on documents


# the superadmin
The superadmin is the highest-level user of the system.
He has full access to the database with the possibility of modifying the data but not deleting the data
He can view all manager and secretary accounts and what they were used for
He can also suspend and delete both the manager and secretary account


## CCSD IMPLEMENTATION
The project was implemented with java for the frontend.
This is because we aim to build a desktop application that can run on any OS
The backend was built using python and the database was done with mysql.
The communication between the java code and the python code was done through the http protocols

# secretary account
only the secretary account was implemented for this project
the various functionalities availble are;
- scan documents
This has 3 functionalities which are;
adding a new citizen to the database,
adding a scanned document of the citizens data into the database,
Searching for citizen's document through their id number
printing back documents to the citizens

- certification of documents
This section was made for the certification of civil status document through digital stamps

- Messaging
This section was made specifically for communication between the managers and the secretaries. since the secretaries have no access to the database or no access to digital stamps. some of those need to be requested directly from the manager hence the messaging section.
It should be noted that each request is already predefined by content and only slight details can be added to it.
NB: This section is in the source code but there are unidentified errors that prevent it from running as a part of the source code hence it is still under development


- Notifcations
This section exist for updates or important info that are sent by the manager or the superadmins to specific or generalsecretaries account

NB: This section is in the source code but there are unidentified errors that prevent it from running as a part of the source code hence it is still under development
