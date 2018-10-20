# Aisera-Programming-Assignment
Instructions on how to solve Aisera JSON assignment 

## Basic Info
This assignment is done in Python 3 on Jupyter Notebook from Anaconda Navigator. To run the whole project, first put the two JSON files under the folder named "data" which is in the same directory of the project IPYNB file or you can put JSON files elsewhere and replace in the code the file path with their actual directory. Then open Anaconda Navigator and open Jupyter Notebook under the environment with Python 3. Finally open and run Aisera_JSON_Assignment_TianyeLin.ipynb at where it is.

## Special Notice
1. To stream and parse JSON files, I am using ijson parser. The reason is each of the given JSON file is a whole object/list of JSON and is not suitable to read line by line as when reading JSON Lines text format. Furthermore, ijson’s parser works efficiently with large JSON files by leveraging generator iterators and yield expressions to lazily load the data instead of reading the whole file in memory .The ijson package could be installed through conda terminal and the document to be referred to is here https://pypi.org/project/ijson/. 

2. The code is orgrnaized modularly. To implement new queries, define query functions under "Define Query Functions" part of the code and call those required query functions in the "Define JSON Sreaming Parsing Function" part. The input parameter of query functions is a list of Python dictionaries.

3. All the parsing and queries are designed specifically for the given JSON files at this moment. For future new JSON files having different format or key-value pairs, modification on code is necessary so as to get the query results.
