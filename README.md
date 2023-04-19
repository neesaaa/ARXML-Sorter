# ARXML-Sorter

## Description
* This program reads an ARXML file containing a list of containers, each with a unique ID, and reorders the containers alphabetically by their "SHORT-NAME" attribute.
* The program then writes the reordered containers to a new ARXML file with the same name as the input file, but with “_mod.arxml” appended to it. For example, if the input file is “Rte_Ecuc.arxml”, the output file should be “Rte_Ecuc_mod.arxml”.
* The name of the arxml file shall be an argument which needs to passed through the command line.
### Exceptions
The program includes Three user-defined exceptions:

* NotVaildAutosarFileException - thrown if the input file is not a valid Autosar file.
* EmptyAutosarFileException - thrown if the input file is empty.
* FileNotFoundException - thrown if the file not found

#### Sample files
* InputSample.arxml: This is a normal ARXML file for testing the normal case.
* emptyFile.arxml: This is an empty ARXML file for testing the empty file case.
* text.txt: This is a Word document for testing the wrong extension case.

### How to Run
1- Clone or download the repository.

2- Open the command prompt or terminal and navigate to the project directory.

3- Run the following commands


```
java -cp bin project.main InputSample.arxml
javac -d bin *.java
java -cp bin project.main <arxml file direction>
```

### Example for last command
```
java -cp bin project.main D:\ARXMLSorter\InputSample.arxml
```
### Batch File
A batch file run.bat is included in the repository to simplify the running of the program. The batch file includes the following cases:

* Normal case - provide the input file and specify its name inside the batch script.
* Not valid Autosar file case - provide the file also.
* Empty file.
  
