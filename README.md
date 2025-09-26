# Notes App (Java)

## Project Overview
**Notes App** is a simple **text-based note manager** written in Java.  
It allows users to:  
1. Add notes  
2. View all notes  
3. Save notes to a file (`notes.txt`)  
4. Read notes from a file  

It uses **Java File I/O (`FileWriter`, `FileReader`, `BufferedReader`)** for storing and reading notes.

---

### File I/O Details

## Saving notes:

  `FileWriter` writer = new `FileWriter`(FILE_NAME, true);

-- true → append mode

-- Adds line separator after each note

## Reading notes:

  `BufferedReader` reader = new `BufferedReader`(new `FileReader`(FILE_NAME));

-- Reads file line by line

## Error Handling:

-- File not found → prompts user to add notes

-- IO errors → prints error message


### Sample Output

   === Notes App ===
1. Add Note
2. View Notes
3. Exit
Choose an option: 1
Enter your note: This semester is my final semester.
Note saved successfully!

=== Notes App ===
1. Add Note
2. View Notes
3. Exit
Choose an option: 2

--- Your Notes ---
- This semester is my final semester.

=== Notes App ===
1. Add Note
2. View Notes
3. Exit
Choose an option: 3
Exiting Notes App...