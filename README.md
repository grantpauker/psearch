# psearch
A program to navigate your project folder <br />
Requirements: <br />
  To run, instead of typing "./psearch", use ". ./psearch", so that it will run in the current bash session <br />
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
  To add autocompletion and an alias for psearch, run the command:
  ```
  echo "alias psearch='. [location-of-psearch-file]'" >> ~/.bashrc && file mv autocomplete /etc/bash_completion.d/psearch
  ```
Usage: <br />
  ```
  psearch [project] | Finds a project with the given name and goes to that directory"
  psearch -l [language] | Lists all projects of a given language, leave blank to just list languages
  psearch -c [language] [project] [file]| Creates a new project in the given language with the given directory name and file name
  psearch -r [project] | Deletes the specified project
  psearch -a [language] | Add a new language folder
  psearch -help | Gives a list of commands
  ```
