## Overview

**CxxHeader2Py** is a powerful Python tool designed to streamline the process of parsing C/C++ header files and extracting valuable information such as defines, enums, structs, and variables. By harnessing the capabilities of **CxxHeader2Py**, developers can effortlessly convert this extracted data into Python objects, saving time and effort in the translation process.


## Usage:
The CxxHeader2Py tool accepts the following arguments:

-a <directory>: Specifies the path to the directory where C/C++ header files are located. CxxHeader2Py will scan the specified directory and its subdirectories to extract the necessary information.

-f <file>: Specifies the path to a specific C/C++ header file. CxxHeader2Py will parse the specified file to extract the required information.

-c <options>: Provides compiler options as common defines. These options are used during the parsing process to ensure accurate extraction of information from the header files.

--version: set the version of the output python file.

-o <output file>: Specifies the path and filename of the output Python file. CxxHeader2Py will generate the Python code with equivalent objects and save it to the specified file.

Example Usage:
```
CxxHeader2Py -a /path/to/headers/ -c "-DOPTION1 -I/path/to/includes" -o output.py --version=1
CxxHeader2Py -f /path/to/header/file.h -c "-DOPTION2 -I/path/to/includes" -o output.py
CxxHeader2Py --version=2
```
