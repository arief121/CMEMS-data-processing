======================================================================
                  SETTING UP PYTHON ENVIRONMENT
======================================================================

This guide provides step-by-step instructions on how to install 
Miniconda on Windows and set up a dedicated Python environment for 
this project using a YAML configuration file.

--------------------------------------------
STEP 1: DOWNLOAD MINICONDA
--------------------------------------------
1. Open your web browser and go to:
   https://www.anaconda.com/download/success
2. Download the Miniconda installer for Windows.

--------------------------------------------
STEP 2: INSTALL MINICONDA
--------------------------------------------
1. Open the downloaded installer file.
2. Follow the installation steps.
3. Wait until the installation is finished.

--------------------------------------------
STEP 3: OPEN ANACONDA PROMPT
--------------------------------------------
1. Click the Windows Start menu.
2. Type "Anaconda" in the search bar.
3. Click "Anaconda Prompt (miniconda3)".
   A terminal window will open.

--------------------------------------------
STEP 4: GO TO YOUR PROJECT FOLDER
--------------------------------------------
In the Anaconda Prompt window, move the
directory to the location of your environment
configuration file:

    cd /path/to/your/folder/

Example:

    cd D:/CMEMS-data-processing/environment/

--------------------------------------------
STEP 5: CREATE THE ENVIRONMENT FROM A YAML FILE
--------------------------------------------
Type the following command:

    conda env create -f <yaml_file.yml>

Example:

    conda env create -f python_envi.yml

Note: replace <yaml_file.yml> with the real
name of your YAML file.

--------------------------------------------
STEP 6: CHECK YOUR ENVIRONMENTS
--------------------------------------------
Make sure the environment was created correctly
by checking the list of environments:

    conda env list

You should see the name of your new environment
in the list.

--------------------------------------------
STEP 7: ACTIVATE THE ENVIRONMENT
--------------------------------------------
To enter the environment, we should activate it:

    conda activate <project_name>

Example:

    conda activate data_processing

--------------------------------------------
STEP 8: OPEN JUPYTER LAB
--------------------------------------------
Run Jupyter Lab:

    jupyter lab

This will automatically open Jupyter Lab
in your default browser.

--------------------------------------------
DONE! Your Python environment is now ready.
You can start running your CMEMS data scripts.
--------------------------------------------
