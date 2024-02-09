# CLI Note-Taking Application

This is a command-line interface (CLI) application built with Node.js that allows you to manage your notes efficiently. You can create, read, update, and delete notes using simple commands.

## Features

- **Create a New Note**: Add a new note with content and optional tags.
- **List All Notes**: View all existing notes.
- **Find Notes**: Search for notes based on a filter term.
- **Remove a Note**: Delete a note by its ID.
- **Launch Web Interface**: Start a web server to view notes in a browser.
- **Clean Database**: Remove all notes from the database.

## Prerequisites

Before running the application, make sure you have the following installed on your system:

- [Node.js](https://nodejs.org/)
- npm (Node Package Manager)

## Installation

To install the CLI note-taking application, you need to follow these steps:

1. **Clone the Repository**: Clone this repository to your local machine using Git:

   ```
   git clone https://github.com/HugoEncinas/notes-cli-app.git
   ```

2. **Navigate to the Project Directory**: Change into the directory of the cloned repository:

   ```
   cd notes-cli-app
   ```

3. **Install Node.js**: Make sure you have at least Node.js version 18.16.0 installed on your system. You can download and install it from [Node.js website](https://nodejs.org/).

4. **Install Dependencies**: Install the required dependencies using npm:

   ```
   npm install
   ```

5. **Link the `note` Command**: To use the `note` command globally, run:

   ```
   npm link
   ```

   This command will create a symbolic link globally, so you can use the `note` command from any directory on your system.

## Usage

To use the CLI note-taking application, follow the instructions below:

1. **Creating a New Note:**

   ```
   note new <note> [-t <tags>]
   ```

   - Replace `<note>` with the content of the note you want to create.
   - Use the optional `-t` or `--tags` flag followed by a comma-separated list of tags to add tags to the note.

2. **Listing All Notes:**

   ```
   note all
   ```

   This command will display all existing notes.

3. **Finding Notes:**

   ```
   note find <filter>
   ```

   - Replace `<filter>` with the search term to filter notes by. This will search for the provided term within the content of notes.

4. **Removing a Note:**

   ```
   note remove <id>
   ```

   - Replace `<id>` with the ID of the note you want to remove.

5. **Launching Web Interface:**

   ```
   note web [port]
   ```

   - Use the optional `[port]` argument to specify the port to bind the web interface. If not provided, the default port is 5000.

6. **Cleaning the Database:**

   ```
   note clean
   ```

   This command will remove all notes from the database.

You can also use the `-h` or `--help` option with any command to view additional information about that command.

## Credits

This CLI note-taking application was built based on the tutorial provided by [Hendrixer](https://github.com/Hendrixer/intro-node-v3).

I would like to express my gratitude to Hendrixer for their comprehensive tutorial, which served as a valuable resource in creating this project.
