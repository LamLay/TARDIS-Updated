**Python version and packages:**
*	Python 3.7 or greater
*	Scikit-learn needs to be 0.20.3 _(recommended)_ up to 0.21.3. Scikit-learn 0.22 or greater will not work. 

**Note:**
If you have this error: _ModuleNotFoundError: No module named 'sklearn.linear_model.base'_ while running the tool, it means you have the incorrect version of scikit-learn. 

**Install:**
*	pip install pydicom            _(The latest version (2.3.0) should work)_
*	pip install pandas
*	pip install numpy
*	pip install spyder-kernels==2.1.1

**Check your python and sklearn versions in cmd/terminal:**
*	python --version
*	conda list scikit

You can **create a virtual environment** in command prompt (cmd) or terminal to run the tool. Here are the instructions: 
1.	pip install virtualenv
2. virtualenv (new environment)          _(example: virtualenv python2)_
3.	cd (new environment)
4. Scripts\activate
5.	conda create -n py37 python=3.7      _(You can install higher version of python)_
6.	conda activate py37
7.	Note: you can now directly install all necessary packages without doing steps 9-12 by using the **requirements.txt** file => Run "pip install -r requirements.txt" in the cmd/terminal. 
8.	python -m pip install scikit-learn==0.20.3     _(scikit-learn version 0.20.3 is recommended)_
9.	pip install pydicom                            _(The latest version (2.3.0) should work)_
10.	pip install pandas
11.	pip install numpy
12.	pip install spyder-kernels==2.1.1             _(Spyder is recommended to run the tool. It should be ≥ 2.1.1 and < 2.2.0)_
  * If there are warnings about _pyqtwebengine_ and _pyqt5_, try: 
    - pip install --upgrade --user pyqtwebengine==5.12.1
    - pip install --upgrade --user pyqt5==5.12.3
13.	python -c "import sys; print(sys.executable)"   _(**Copy the path** returned by this command)_
14.	conda deactivate              
15.	spyder 			

If you still cannot open the Spyder, close and reopen the cmd/terminal and then try:
*	cd <new environment>          
*	spyder

In Spyder, go to **Preferences > Python Interpreter > Use the following interpreter**, and _**paste the path**_ copied from the terminal into the text box. You can now use the tool in a virtual environment. 
