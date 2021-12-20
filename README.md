# TARDIS (v2)
## Artificial Intelligence Powered Prediction for Online Adaptive Patient Specific QA ## 

### A Tool for Approximating Radiotherapy Delivery via Informed Simulation (TARDIS) ###
This is the update of Chuang's project: https://github.com/k1a2i3oscar/TARDIS#a-tool-for-approximating-radiotherapy-delivery-via-informed-simulation-tardis

Tutorial:

* Download all files. It is recommended to have the models, the scaler.plk files, and the tool.py in the same folder. 
* Open the tool.py with Python platform and run the script. 
* At GUI, input desired DICOM-RT plan by clicking "Open" button.  
* Decide what type of MLC errors you want to predict. The tool can predict 3 types of MLC errors:
  * Delivery error at the machine
  * Conversion error from DICOM-RT to deliverable trajectory
  * Combined error - sum of delivery error and conversion error 
* Choose one machine learning model based on treatment technique (IMRT or VMAT). Then run the tool.  
* When the prediction process is completed, the tool will automatically generate a new DICOM-RT with predicted MLC positions, and command separate values (CSV) files including mechanical parameters and predicted MLC errors and positions for individual field/arc. 
* Re-import the new DICOM-RT into treatment planning system to evaluate the change in dose. 

For research or academic purposes. Not intended for clinical use. 
For researchers, any publication using this tool please cite the accompanying paper 
“Lay, Chuang, Adamson, Giles, A Tool for Patient Specific Prediction of Delivery Discrepancies in Machine Parameters Using Trajectory Log Files, 2020"

The copyrights of the software and contents are owned by Duke University and are made available for academic purposes only. Outside contributions to the Duke-owned code base and contents cannot be accepted unless the contributor transfers the copyright to those changes over to Duke University.

To enter a license agreement, please contact the Duke Office of Licensing and Ventures at olvquestions@duke.edu with reference to “OLV File No. 6733” in your email.

This software is distributed AS IS, WITHOUT ANY WARRANTY; and without the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.

 
