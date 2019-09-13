---
title: "Introduction to BIDS-EEG"
teaching: 0
exercises: 0
questions:
- "How do I get my data into a BIDS standard?"
objectives:
- "Understand how to initialize your data into a BIDS standard.
keypoints:
- "Your data will be initialized and in a BIDS standard and are now ready to be submitted to the Lossless pipeline."
---

## Initializing Data

1. Download Face13 sourcedata folder from [here](https://drive.google.com/drive/folders/1xq85woDpAYXhCtzdgjkXpjjjggiWSKtc)

2. Create a project folder (for the tutorial we will call this folder 'Face13'). This can be done in a terminal window: 

    ```bash
    >> mkdir Face13
    ```

3. Move the `sourcedata` folder into this project folder.

4. Change directory into the Face13 folder:

    ```bash
    >> cd path/to/project/directory/Face_13/
    ```

5. Create a code folder within the project folder:

    ```bash
    >> mkdir code
    ```

6. Change directory into the code folder:
    
    ```bash
    >> cd code
    ```

7. Within the code folder, clone the BIDS initialization suite:

    ```bash
    >> git clone --recursive https://github.com/BUCANL/BIDS-Init-Face13-EEGLAB.git
    ```

8. Open MATLAB and navigate to your project directory to make it your current path. 

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

{% include links.md %}

