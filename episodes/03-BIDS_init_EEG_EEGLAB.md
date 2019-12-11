---
title: "Initializing Data into the BIDS Standard"
teaching: 0
exercises: 0
questions:
- "How do I get my data into the BIDS standard?"
objectives:
- "Understand how to initialize your data into the BIDS standard."
keypoints:
- "Your data will be initialized into the BIDS standard and is ready to be submitted to the Lossless pipeline"
---

## Initializing Data

1. Download Face13 sourcedata folder from [here](https://drive.google.com/drive/folders/1xq85woDpAYXhCtzdgjkXpjjjggiWSKtc). The whole `sourcedata` folder needs to be downloaded.

2. Create a project folder in the location that you would like to work from (for the tutorial we will call this folder 'Face13'). This can be done in a terminal window: 

    ```bash
    >> mkdir Face13
    ```

3. Move the `sourcedata` folder into this project folder.

4. Change directory into the Face13 folder:

    ```bash
    >> cd Face13
    ```

5. Create a code folder within the project folder:

    ```bash
    >> mkdir code
    ```

6. Change directory into the code folder:
    
    ```bash
    >> cd code
    ```

7. Within the code folder, clone the BIDS initialization suite. **NOTE:** Use the recursive flag in order to clone all the required submodules:

    ```bash
    >> git clone --recursive https://github.com/BUCANL/BIDS-Init-Face13-EEGLAB.git
    ```

8. Open MATLAB and navigate to your project directory (Face13 directory) to make it your current path. 

9. In the MATLAB command window type:

    ```matlab
    >> addpath code/BIDS-Init-Face13-EEGLAB
    >> addpath code/BIDS-Init-Face13-EEGLAB/eeglab
    >> eeglab
    ```

10. To merge and relabel bdf files run the `init_script.m` in the MATLAB command window: 

    ```matlab
    >> init_script
    ```

11. To BIDSify the data run the `bids_face13.m` script in the MATLAB command window:

    ```matlab
    >> bids_face13
    ```
12. A file chooser window will pop up when running the `bids_face13.m` script. Select the **project directory** with the file chooser. 

13. Once this procedure is completed, your initialized data will be in the BIDS standard (`sub-*/eeg/`) in the root of your project folder. 

{% include links.md %}

