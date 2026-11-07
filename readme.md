This will be a note-taking app to help people organize their thoughts, leave reminders for themselves, write down
information for later, etc. <br>
Planned features: <br>
-Create/edit/delete "notes", where users can input text and images <br>
-Organize notes in "folders" <br>
-Save what they've written so they can view it later <br>
-Search their saved notes for specific words/phrases <br>
-Optional account creation to allow viewing of notes across multiple devices <br>
-Save note to device as a PDF <br>

Entity-Relationship Diagram (ERD) to show the different entities involved in the project, their attributes, and their
relationships to each other
<img width="1142" height="509" alt="image" src="https://github.com/user-attachments/assets/b3fb2f7d-a1e3-4a35-9ca6-e9114011f192" />

Relational schema diagram to show how the database will be structured
<img width="861" height="672" alt="image" src="https://github.com/user-attachments/assets/7e9f5a4b-a396-4844-8322-1f837814db6f" />

--Database Implementation--
For this project, I used MariaDB since I was already familiar with it from a previous class. I created three tables for my
database, "Account", "Note", and "Folder". These entities reference each other for several attributes, so it made sense to
me to create all three to start. Both the Folder and Note tables have an AccountID foreign key referencing the AccountID field 
in the Account table. Additionally, the Note table references the FolderName field of the folder table and the Folder table
references the Title field of the Note table.

