# Author Accounts

## How its implemented
Currently author accounts are in the early stages.
Right now there is a custom group called Author Accounts.
This group has the change author, and view author permissions.
Those two permissions are default in django.
However, on the backend there is a custom database object called `AuthorAdminPermission'.
This maps an individual admin account to one or more author objects in the database.
Then there is logic to make it so that each of these user accounts can only see and edit the specific author profiles they have been assigned.
Notably no author account has the ability to delete any author object.

## Getting an account set up
Message the current tech lead on discord.
Tell them your Andrew id, and what characters you have written under.
They will give you a username and default password.
Log in and change your password.
You can then click on the Authors tab and see a list of all of the authors that you have the ability to edit.
If you start writing under a new character message the tech lead and they can add that additional character to your profile.