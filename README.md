📔 Personal Journal Application
A lightweight, terminal-based journal manager built with Python. This application uses Object-Oriented Programming (OOP) to handle daily entries, store them permanently in a text file, and allow for easy retrieval through search.

🚀 Key Features
Persistent Storage: Entries are saved to journal.txt so they remain even after the program closes.

Auto-Timestamping: Every entry is automatically stamped with the date and time.

Search Functionality: Quickly find past thoughts using keywords.

Error Handling: Uses try...except blocks to prevent crashes if files are missing or permissions are denied.

🛠️ Technical Breakdown
Core Modules
os: Used for file system operations, specifically for deleting the journal file.

datetime: Used to generate real-time timestamps for each entry.

Program Logic
The application is structured using a JournalManager class, which encapsulates all major operations:

__init__: Initializes the file name and prepares the system.

add_entry: Appends new text to the journal without deleting old data.

view_all_entries: Reads and displays the entire history of the journal.

search_entry: Filters entries by a user-provided keyword.

delete_all_entries: Removes the journal file from the disk after user confirmation.
📝 Example Output
Plaintext
--- MENU: 1:Add | 2:View | 3:Search | 4:Delete | 5:Exit ---
Choice: 1

What's on your mind today?
> Today I learned about file handling in Python.
Done! Entry saved.
🛡️ Safety Features
The code includes robust error handling to ensure a smooth user experience:
FileNotFoundError: If you try to view an empty journal, the app informs you rather than crashing.
PermissionError: Notifies you if the file system is locked.
Confirmation Prompt: Prevents accidental deletion of your entire journal history.

https://drive.google.com/file/d/1XSGX7z6zX2ZyfR8XHTygzxsxKBO6Z3I7/view?usp=drive_link
