# Student Record Manager

A console-based Java application to manage a simple student roster — add, remove, and search students by name, with export to a text file.

## Features

- **Add Student**: Add a new name to the roster
- **Remove Student**: Remove a student by name
- **Search Student**: Search for a student and view their roll number
- **Export**: Save the current roster to `Student.csv`

## Tech Used

- Java
- `Scanner` for console input
- `FileWriter` for file export

## How to Run

```bash
javac Test.java
java Test
```

Follow the on-screen menu to choose an operation.

## Project Structure

- `Test.java` — contains the data/roster logic, the input-handling layer, and the menu, split across `Test100`, `Child3`, and `Option` classes

## Notes

Roll numbers are derived from list position, so they shift if a student is removed. The exported file uses space-separated values rather than true comma-separated CSV — update `Csv()` if a real CSV format is needed downstream.

## Future Improvements

- Wrap the menu in a loop so multiple operations can run in one session
- Switch export format to proper comma-separated CSV
- Add input validation for menu selection
- Assign persistent roll numbers instead of deriving from list index
