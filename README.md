# filesearch-dir
search in term "text" in a specific directory written in python  
Let’s break down the purpose and function of the provided code:

Objective:
The code is designed to search for a specified term within various types of files (CSV, TXT, DOCX, XLSX, ACCDB) located in a given directory.
It uses parallel processing (via ProcessPoolExecutor) to improve efficiency when searching multiple files simultaneously.
Functions Explained:
search_in_csv_chunk(file_path, search_term):
Reads a CSV file in chunks (to manage memory efficiently).
Filters rows where the specified search term exists.
Returns the filtered rows as a list.
search_in_txt_chunk(file_path, search_term):
Reads a text file line by line.
Appends lines containing the search term to the results list.
search_in_docx_chunk(file_path, search_term):
Reads a DOCX (Microsoft Word) file.
Extracts text from paragraphs.
Appends paragraphs containing the search term to the results list.
search_in_xlsx_chunk(file_path, search_term):
Reads an XLSX (Excel) file.
Iterates through rows and cells.
Appends rows containing the search term to the results list.
search_in_accdb_chunk(file_path, search_term):
Connects to an Access database (ACCDB file).
Returns the query results.
search_files_parallel(directory, search_term):
Walks through the specified directory.
For each file, submits the appropriate search function based on the file type.
Collects and returns the search results.
Example Usage:
The example usage section demonstrates how to apply the search to a specific directory ('/currect_directory') with the search term 'write the term you want to search in currect dir'.
It prints the results for each file found

follow me in the instagram "@esefkh740_"
