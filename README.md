# B-LacKineticTraceAnalyzer_04-10-2008

Date Written: 04/10/2008

Industry: Medical Device Manufacturer

Device: Blood Analyzer

Platform: Lactate Sensor

GUI:
The “Lactate_Logfile_Macro_rev B.xls” file contains the GUI.

Sample Raw Data File (log file):
LOG1155.A08 – A text file with tab delimiters.

Sample Output:
The “691498_B-Lac Analysis.xls” file is an example of the output.

Application Description:
This program mines spectrometry data from a text file (log file) dumped from the blood analyzer then plots the second 
derivative of the % transmittance to calculate lactate concentration in a given blood sample.  The log files contains 
the communication between all the instrument firmware as well as the raw spectrometry data.  The raw data always followed 
specific firmware commands.  However, the quantity and location of the data varies.  So a simple algorithm was written 
to find the data and determine how much data was there.  This information would determine how the resulting excel file 
was built.  Since this data analysis tool was used in early R&D stages of the instrument development, no effort was made 
to create a robust GUI.  The output files are highly complex, but aesthetically formatted excel files containing no less 
than 21 worksheets.  The number of worksheets is dependent on the quantity of data in the log file.  The formatting 
streamlined data interpretation and report generation. 
