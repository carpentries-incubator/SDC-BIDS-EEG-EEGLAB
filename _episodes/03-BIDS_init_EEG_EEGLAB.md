---
title: "Initializing Data into BIDS"
teaching: 0
exercises: 0
questions:
- "How do I get my data into a BIDS compliant folder structure?"
objectives:
- "Understand how to initialize your data into BIDS."
keypoints:
- "Your data will be initialized into the BIDS standard and is ready to be submitted to the Lossless pipeline"
---

## Initializing Data

1. Download Face13 sourcedata folder from [here](https://drive.google.com/drive/folders/1xq85woDpAYXhCtzdgjkXpjjjggiWSKtc). The whole `sourcedata` folder needs to be downloaded.

2. We need to create the project folder where we will be working in throughout this tutorial. For this tutorial we will call this folder 'Face13'. Make this folder in a location that is convient and easy to navigate to such as on your Desktop. Making this folder can be done in a terminal window using the following command:

    ```bash
    >> mkdir Face13
    ```

3. To begin working with the sample dataset, move the `sourcedata` folder into this `Face13` project folder. It is important that the bdf task files are located in the `sourcedata/eeg` folder so that the initalization script is able to locate the files.

4. In the terminal window, change directory into the Face13 folder:

    ```bash
    >> cd Face13
    ```

5. Create a code folder within the project folder:

    ```bash
    >> mkdir code
    ```

    We will download the BIDS initialization suite into this `code` folder. The BIDS initialization suite contains a version of EEGLAB as well as the scripts that are necessary to initialize our raw data for preprocessing and organize our data into a BIDS compliant folder scructure. 

    In line with the BIDS specification, the `code` folder in the root of our project folder will store the source code of scripts that are used to prepare the dataset.

6. Change directory into the code folder:
    
    ```bash
    >> cd code
    ```

7. Within the code folder, clone the BIDS initialization suite. **NOTE:** Use the recursive flag in order to clone all the required submodules:

    ```bash
    >> git clone --recursive https://github.com/BUCANL/BIDS-Init-Face13-EEGLAB.git
    ```
    It is important that the initalization suite is cloned into the `code` folder within your `Face13` project folder because we will have to let Matlab know where in our path EEGLAB is located.

    Once we have the BIDS initalization suite and the sample dataset downloaded, we are ready to open Matlab and begin the initalization process.

8. Open MATLAB and navigate to your project directory (Face13 directory) to make it your current path. 

9. Before we can open EEGLAB, we have to add it to our path. In the MATLAB Command Window type:

    ```matlab
    >> addpath code/BIDS-Init-Face13-EEGLAB
    >> addpath code/BIDS-Init-Face13-EEGLAB/eeglab
    ```

10. To open EEGLAB, in the MATLAB Command Window type:

    ```matlab
    >> eeglab
    ```

    For initalization and BIDSifying our data we will run two scripts by typing the script names in the Command Window. We will not be using the EEGLAB GUI directly, but we still have to add EEGLAB to our path because our scripts will call EEGLAB functions.

11. The first script we will run is the `init_script.m`. This script will load our raw data files (bdf files for the Face13 dataset) and merge the multiple task files for each subject into a single file. This script also relabels events for future processing. 

    To run the `init_script.m` in the MATLAB Command Window type: 

    ```matlab
    >> init_script
    ```
    The output of the `init_script` is a single set file for each participant. These files will be saved within the `sourcedata/eeg` folder. 

12. Now that our data is initalized, the next step is to organize it in a BIDS compliant folder structure. This will result in each subject having their own folder that contains an `eeg` folder to store all of the EEG files for that participant. 

    To BIDSify the data, run the `bids_face13.m` script in the MATLAB Command Window:

    ```matlab
    >> bids_face13
    ```
13. A file chooser window will pop up when running the `bids_face13.m` script. This file chooser is asking where you want the sub-*/eeg folders to be created. Select the **project directory** (Face13 folder) with the file chooser. 

    Creating the sub-*/eeg folders in the root of your project directory will create a folder structure that looks like this:
    
    ![BIDS Folder Structure]({{ page.root }}/fig/bids_folders.png)

    Several files will be produced within each `sub-*/eeg/` folder. All of the file names contain the subject number as well as the task name and a suffix to denote the infromation that is saved within that file. For example, the EEG recording data files have a suffix of `_eeg` and are saved as .edf files. There is also a Sidecar JSON file that has an `_eeg` suffix and a .json extension. The JSON file contains relevant metadata that is important to be stored in an accessible location.

14. Once this procedure is completed, your initialized data will be in the BIDS standard (`sub-*/eeg/`) in the root of your project folder. 

{% include links.md %}

