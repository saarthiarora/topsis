TOPSIS Implementation in Python
Course: UCS654 - Predictive Analytics using Statistics
Assignment: Assignment-1 (TOPSIS)
Author: Saarthi Arora
Roll Number: 102303457

About the Project
This repository contains a Python implementation of the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method. TOPSIS is a multi-criteria decision-making (MCDM) technique used to rank multiple alternatives based on their distance from the ideal best and ideal worst solutions.

Installation - USER MANUAL
Topsis-Saarthi-102303457 requires Python 3 to run. The following dependencies will be installed automatically with the package:pandasnumpyPackage on PyPI
You can find this package at: https://pypi.org/project/Topsis-Saarthi-102303457/Install via pip
pip install Topsis-Saarthi-102303457
UsageOnce installed, you can run the program directly from your command prompt/terminal using the following syntax:
Bashtopsis <inputFile> <weights> <impacts> <outputFile>
Parameters:
ParameterDescriptioninputFilePath to the source CSV or Excel file (must have 3+ columns) weights
Comma-separated numeric values (e.g., "1,1,1,1")impactsComma-separated symbols + for benefit or - for cost (e.g., "+,+,-,+")outputFileName of the file where results will be saved
Example:
topsis sample.csv "1,1,1,2,1" "+,+,-,+,+" result.csv
Input File Format
The input file must follow these constraints:
The first column should contain the names of the alternatives (e.g., Model names).
The second column to the last column must contain numeric values only.
The file must contain at least 3 columns in total.
Error Handling
The package includes comprehensive error checking for:
Argument Count: Ensures exactly 4 parameters are provided.File Existence: 
Validates if the input file exists.Data Types: Checks that all criteria columns are numeric.
Mismatch: Ensures the number of weights, impacts, and columns are identical.
Impact Symbols: Only allows + and -.

License© 2026 Saarthi. Distributed under the MIT License.
