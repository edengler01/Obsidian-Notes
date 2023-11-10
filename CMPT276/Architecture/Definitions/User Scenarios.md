# Example
##### Initial Assumption
- A user is looking for a book based off of book name, book author, course code that is was associated with it, book condition, and price of the book. They are already authenticated. 


##### Normal
- The user chooses to search for a book based of the criteria. They are prompted enter the criterion they want seach off of. The input is then sent off to the server. 

- On completion, the system will show the user all the books that are relevant to the criterion that they put. 
##### What Can Go Wrong
- A user can input malicious code that could give them access to senstive, but encrypted information.

- A user can input malicous code that could break the integrity of the database.

##### System State on Completion
- User is logged in. The server will display all the books that student is interested in.