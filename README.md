# fluorescent-trace-analysis-in-Python
This is a collection of Python functions that do the following for fluorescent trace
(imaging data) output from Fiji:

The traces (stored in csv files) are read into Python. The following processing is performed:
1) bg subtraction
2) each trace (representing a single roi or region of interest) is examined to pick out "peaks" (spontaneous exocytosis events) represented by a sudden increase in flourescence. This involves implementation of a threshold
3) the performance of different thresholds can be tested automatically (false positives and false negatives against a curated set
   of data)  
4) once a threshold has been picked the events for different conditions can be averaged and graphed
5) the sorted traces can be written to Excel

Because this is a collection of functions that together complete the goal task I've created a mock "run_client" file that
demonstrates the order that the functions should be run as well as the Python libraries used 

