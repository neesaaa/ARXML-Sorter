# ARXML-Sorter

## Description
* This program reads an ARXML file containing a list of containers, each with a unique ID, and reorders the containers alphabetically by their "SHORT-NAME" attribute.
The program then writes the reordered containers to a new ARXML file with the same name as the input file, but with “_mod.arxml” appended to it. For example, if the input file is “Rte_Ecuc.arxml”, the output file should be “Rte_Ecuc_mod.arxml”.
The name of the arxml file shall be an argument which needs to passed through the command line.
