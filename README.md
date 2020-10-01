# Phonebook_Bash_Script_Linux

## Summary:
The goal of this script is to creates a phonebook on your system that contains a list of your contact names and numbers, with these features:

- Script can take options, e.g. "phonebook -v"
- When running the script without options, it will print the phonebook available options.
- Normally there is a “.phonebookDB.txt” which ur script creates to store the names and numbers. 
- the database inside the script itself (meaning the script would edit itself while running), that would make it highly portable.
- a single name can have multiple phone numbers within the same database entry.
- The script checks if a database file exist before trying to create a new one

## The available options are:

- Insert new contact name and number, with the option "-i"
- View all saved contacts details, with the option "-v"
- Search by contact name, with the option "-s" 
- Delete all records, with "-e"
- Delete only one contact name, with "-d"

**Common bugs you need to take care of:**

- use defensive coding strategy to counter wrong user inputs
- The inputs will contain names with similarities ( e.g. “ahmed ali”, “ali ahmed”, “Ali Ali”  etc)(which to delete ?!)
