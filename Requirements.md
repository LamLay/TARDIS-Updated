**Python version and packages:**
•	Python 3.6 or great
•	Scikit-learn needs to be 0.20.3 (recommended) up to 0.21.3. Scikit-learn 0.22 or greater will not work. 
- If you have this error: ModuleNotFoundError: No module named 'sklearn.linear_model.base' while running the tool, it means you are not having the correct version of scikit-learn. 

**Install:**
•	pip install pydicom            # The latest version (2.3.0) should work
•	pip install pandas
•	pip install spyder-kernels==2.1.1

**Check your python and sklearn versions in cmd/terminal:**
•	python --version
•	conda list scikit

You can **create a virtual environment** in command prompt (cmd) or terminal to run the tool. Here are the instructions in cmd/terminal: 
•	pip install virtualenv
•	virtualenv <new environment>          # example: virtualenv python2
•	cd <new environment>
•	Scripts\activate
•	conda create -n py37 python=3.7      # You can install higher version of python
•	conda activate py37
•	python -m pip install scikit-learn==0.20.3     # scikit-learn version 0.20.3 is recommended
•	pip install pydicom
•	pip install pandas
•	pip install spyder-kernels==2.1.1       # Spyder should be ≥ 2.1.1 and < 2.2.0
•	if there are warnings about pyqtwebengine and pyqt5, try: 
o	pip install --upgrade --user pyqtwebengine==5.12.1
o	pip install --upgrade --user pyqt5==5.12.3
•	python -c "import sys; print(sys.executable)"   # **Copy the path** returned by this command
•	conda deactivate              
•	spyder 			# Spyder is recommended to run the tool

If you still cannot open the Spyder, close and reopen the cmd/terminal and then try:
•	cd <new environment>         
•	spyder

In Spyder, go to **Preferences > Python Interpreter > Use the following interpreter**, and paste the path copied from the terminal into the text box. You can now use the tool in a virtual environment. 
