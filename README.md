# psearch
A program to navigate your project folder <br />
Requirements: <br />
  Initialize psearch by running the install file as follows:
  ```
  chmod +x ./install
  ./install
  ```
  Also, you projects folder should be in this format: <br />
  <pre>
    └── [project-folder]
        ├── [language1]
        |   ├── [file1]
        |   └── [file2]
        ├── [language2]
        |   ├── [file1]
        |   ├── [file2]
        |   └── [file3]
        └── [language3]  
            └── [file1]</pre>

Usage: <br />
  ```
  psearch [project] | Finds a project with the given name and goes to that directory"
  psearch -l [language] | Lists all projects of a given language, leave blank to just list languages
  psearch -c [language] [project] [file]| Creates a new project in the given language with the given directory name and file name
  psearch -a [language] | Add a new language folder
  psearch -r [project]  | Deletes the specified project
  psearch -b [project]  | Backsup your project folder

  psearch -help | Gives a list of commands
  ```
