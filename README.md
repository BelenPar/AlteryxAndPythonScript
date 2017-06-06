# AlteryxAndPythonScript
How to run a Python Script in Alteryx. 

To run a python script in Alteryx we can use the Run Command Tool:
 

This is an example for v10.6 of Altery, using the run command tool to execute a Python script in the Designer and use its output in the workflow. This kind of sripts can be very useful for the dataprocessing and things like that:

First open Run Cimmand
![alt text](https://github.com/BelenPar/AlteryxAndPythonScript/blob/master/RunCommand.png)

To use a Python script the Command must be Python.exe. I would suggest to use the full path to be sure that the Python interepreter used is the one that you want (in case you are useing more than one interpreter).
In Command Arguments it's needed the full path to the Python script.

The tricky part is to dump the data that is currently in Alteryx to a file so that your script can read.

The Read Results should point to a file written by the Python script. Alteryx will use that file like the input to the flow.
