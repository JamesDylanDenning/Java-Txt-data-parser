Text File Data Parser - CCUL

•	Developed in house application for financial and accounting team to streamline workflow and auditing processes

•	Integrated application saving the client 5-10 hours each month by automating manual data entry and revision process

•	Java programming fundamentals while maintaining software development and cybersecurity best practices





Features
File Selection: Users can select multiple files at once for processing, allowing for batch operations and improved efficiency.

Data Extraction: The application searches for specific patterns in the text, such as total transaction fees and deductions, to compute and extract financial data.

Custom Output File Naming: Users can specify the name of the output file where the consolidated data will be saved. If no name is provided, a default name is used.

Real-time Feedback: The application provides real-time feedback through a text area within the GUI, displaying the status of file processing, including any found data and calculation results.

Error Handling: Basic error handling is implemented, with error messages displayed in the GUI's text area, ensuring users are aware of any issues during processing.





Technologies Used
Java Swing: For creating the graphical user interface (GUI), enabling user interaction with the application.

Java IO: For file handling operations, including reading from and writing to files.

Regular Expressions: To identify and extract specific patterns of data within the text files.






Key Components
JFrame, JButton, JTextField, JTextArea, JScrollPane, JLabel, JPanel: Swing components used to build the application's interface.

FileReader, BufferedReader, FileWriter, BufferedWriter, PrintWriter: Classes from the Java IO package for reading and writing files.

Pattern, Matcher: Classes from the java.util.regex package to search for and extract data based on predefined patterns.






Functionality
GUI Initialization: On application start, the GUI is initialized with a frame containing a button to select files, a text field for the output file name, and a text area for feedback.

File Selection and Processing:
Upon clicking the "Select Files" button, a file chooser dialog allows the user to select multiple files.

The application reads each selected file, looking for specific data points using regular expressions. 

The primary focus is on extracting "TOTAL TRANS FEE INCOME" values and other related financial data.

It computes a final value by applying calculations on the extracted data and logs the process in the GUI's text area.

Output File Generation:
A new output file is created (or appended if it already exists) where the processed data is saved in a structured format.

The first line of each file is processed to extract a specific piece of information, which, along with the calculation results, is written to the output file.

Java SE Development Kit 21.0.2

https://www.oracle.com/java/technologies/javase/jdk21-archive-downloads.html
