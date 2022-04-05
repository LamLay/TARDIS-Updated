# TARDIS (v2)
## Artificial Intelligence Powered Prediction for Online Adaptive Patient Specific QA ## 

### A Tool for Approximating Radiotherapy Delivery via Informed Simulation (TARDIS) ###
This is the update of Chuang's project: https://github.com/k1a2i3oscar/TARDIS#a-tool-for-approximating-radiotherapy-delivery-via-informed-simulation-tardis

**Instructions:**

* Download and unzip all files and folders. 
* If you plan to use the _bagged tree models_ later, convert them from .rar files into .sav files. 
* Instructions to obtain the correct Python version and packages are provided in the **Requirements.md** file. 
* Open the **tools_AllErrors.py** with a Python platform and run the script. 
* At GUI, click the "Open" buttons to input desired DICOM-RT plan, select folders that have the machine learning models and scaler.pkl files. 
* Select the output folder where you want to save the new DICOM-RT plan, which is the output of the tool.
* Type the name of the output file in the textbox in GUI.   
* Decide what type of MLC errors you want to predict. The tool can predict 3 types of MLC errors:
  * Delivery error at the machine
  * Conversion error from DICOM-RT to deliverable trajectory
  * Combined error - sum of delivery error and conversion error 
* Choose one machine learning model based on treatment technique (IMRT or VMAT). 
* Run the tool by clicking the "Run" button.  
* When the prediction process is completed, the tool will automatically generate a new DICOM-RT plan with predicted MLC positions, and command separate values (CSV) files including mechanical parameters and predicted MLC errors and positions for individual field/arc.  
* Re-import the new DICOM-RT plan into a treatment planning system to evaluate the change in dose. 

**Note:** 
* There will be an error when an IMRT DICOM plan is input into a VMAT model because an IMRT DICOM doesn’t have any information about gantry rotation. In this case, a message box will appear and the program will stop running. 
* A VMAT plan has all information needed in an IMRT plan, so the script will produce no error if a VMAT DICOM is input into an IMRT model. The user should make sure that the input plan is indeed a VMAT plan before using a VMAT model to predict MLC errors. 
* The bagged tree models need to be converted into .sav files before using the tool. If the user tries to use a bagged tree model before the conversion, a message box will appear and the program will stop running.

For research or academic purposes. Not intended for clinical use. 
For researchers, any publication using this tool please cite the accompanying paper 
“Lay, Chuang, Adamson, Giles, A Tool for Patient Specific Prediction of Delivery Discrepancies in Machine Parameters Using Trajectory Log Files, 2020"

The copyrights of the software and contents are owned by Duke University and are made available for academic purposes only. Outside contributions to the Duke-owned code base and contents cannot be accepted unless the contributor transfers the copyright to those changes over to Duke University.

To enter a license agreement, please contact the Duke Office of Licensing and Ventures at olvquestions@duke.edu with reference to “OLV File No. 6733” in your email.

This software is distributed AS IS, WITHOUT ANY WARRANTY; and without the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

 
