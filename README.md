# Roulette

_Purpose_ : This document shows you how to insert many boards easily.

## What is a board template ?

A board is defined by 3 free zoom zones :
- 1 Free Zoom Zone including :
	An image
	Some text
- 1 Free Zoom Zone including :
	3 issues linked to 7 actions
	2 issues linked to another boards
- 1 New Kanban including :
	10 users
	8 step WIP
	1 Backlog column
	1 Done column
	80 stickies whose 10 in the backlog column and 70 dispatched between users
   
## Configuration from scratch

### Install the database scheme

Steps to following :
- Retrieve the project on gitlab : URL
- Create a new database in PgAdmin
- Open the "liquibase.properties" file and configure your database url, username, password...
- Open the "init-user.xml" file and change the value in the property tag called 'user'
- Run init-database.sh executing the command : $ ./init-database.sh

### Insert boards in the database

Steps to following :
- Run init-data-boards.sh executing the command : $ ./init-data-boards.sh user count

Now, you have a user who have n different boards with the sceme described above.










