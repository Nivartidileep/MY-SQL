TRANSACTION: THE PROCESS OF COMBAINING ALL RELATED OPERATIONS INTO A SINGLE UNIT AND EXECUTING THEN ACCORDING TO THE RULE "EITHER ALL OPERATIONS SHOULD SUCCEED OR NONE SHOULD SUCCEED" IS CALLED TRANSACTION MANAGEMENT.



A TRANSACTION IS CONSIDERED A SINGLE UNIT OF WORK AND FOLLOWS THE PRINCIPLE "EITHER ALL OR NONE"



EXAMPLE:

FUNDS TRANSFER

CONSIDER A MONEY TRANSFER

=============

PROPERTIES:

\---------

ATOMESITY

\--------

\->ALL OR NOTHING.

COSISTANTCY

\-----------

\->THE DATABASE REMAINS IN A VALID STATE.

ISOLATION

\---------

\-> TANSACTIONS DO NOT INTERFACE WITH EACH OTHER.

DURABILITY

\----------

\-> COMMITED CHANGES ARE PETMINENET.



\----------------------------------------

TYPES:

1\) LOCAL TRANS

\---------------

=> TRANSCATIONS ALL OPERATIONS OF A TRANSACTION ARE EXECUTED ON THE SAME DATABASE.

EX:

FUNDS TRANSFER FROM ONE ACCOUNT TO ANOTHER ACCOUNT WHERE BOTH ACCOUNTS ARE SAME BUT SAME BANK.

2\) GLOBAL TRANS

\---------------

=> TRANSCATIONS ALL OPERATIONS OF A TRANSACTION ARE EXECUTED ON THE DIFFRENT DATABASE.

EX:

FUNDS TRANSFER FROM ONE ACCOUNT TO ANOTHER ACCOUNT WHERE BOTH ACCOUNTS ARE SAME BUT DIFFRENT BANK.

==========================================================================================================================

TCL(TRANSCATION CONTROL LANGUAGE)

\----------------------------------

\->COMMIT (NOT MODIFICATION)

\--------------------------------

=> COMMIT  IS USED TO PERMENANTLY SAVED ALL CHANGES MADE DURING  THE CURRENT TRANSACTION INTO THE DATABASE.



ONCE COMMITTED.



&#x09;CHANGES BECOME PERMANANT.

&#x09;OTHER USERS CAN SEE THE CHANGES.

&#x09;YOU CANNOT UNDO THE CHANGES USING ROLLBACK.



\->ROLLBACK (UNDO OPERATION - INFORMATION BACK)

\-----------------------------------------------------

=> ROLLBACK IS USED TO UNDO ALL CHANGES MADE IN THE CURRENT TRANSACTION BEFORE A COMMIT.

IF SOMETHING GOES WRONG. ROLLBACK RESTORES THE DATABASE TO ITS PREVIOUS STATE.



\->SAVE-POINT

\------------

=>



Introduction to stored procedures

=================================

a stored procedure is a named, precompiled collection of one or more sql

statements that is stored inside the database and can be executed called whenever reqired. instead of sending the application simply call it.



why used:

1.performance

2.reusablity

security

redued n\\w traffic

maintainability

consistency



advantages

\--------------

faster excecution after completion.

reduced duplicate sql

supports transcation,loops,condtions,variables.....ect.

easy maintanence



disadvantages

\--------------

debugging can be difficult.

vendor specific syntax.

complex procedures may become hard to maintain.



syntax to create stored procedure



DELIMITER //

CREATE PROCEDURE procedure\_name()

BEGIN

\------sql statements

END //

DELIMITER;



IN Parameter

\------------

an IN Parameter is used to pass a value into a stored procedure.

the procedure can use the



OUT Pararmeter

\--------------

An out parameter is used to return a value from the stored procedure to the caller.



==========================================================================================================================









































































































&#x20;

