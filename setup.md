---
title: Setup
---

### Download and install Matlab

You will need a fairly recent version of Matlab (procedure tested on Matlab 2012b and newer versions). For detailed installation instructions, click [here](https://www.mathworks.com/help/compiler/install-the-matlab-runtime.html).

### Obtain lesson materials

1. Download the Face13 tutorial dataset from this [google drive](https://drive.google.com/file/d/1AWgN0DOstCw7UB5puxHL_beddNzPZ__v/view?usp=sharing). 
2. Download the initalization suite from this [google drive](https://drive.google.com/file/d/1p1OCsOdu27Tg_QYhNx_mJIkNm3ygyekr/view?usp=sharing)
3. Create a folder called `Face13` on your Desktop.
4. Move the downloaded folders to `Face13`.
5. Unzip the folders. 

You should see two folders called `sourcedata` and `code` in the `Face13` directory on your Desktop. The `sourcedata` folder contains the EEG data and standard montages that are used during initialization. The `code` folder contains a version of EEGLAB and the necessary scripts to intialize the data into a BIDS compliant folder structure.

Your `Face13` folder should look like this:
![Setup folder structure]({{ page.root }}/fig/setup_folderlayout.png)

> ## Important Note
> It is important that your `Face13` folder is organized in this way so that Matlab and the provided code are able to locate files. 
> 
> {: .source}
{: .callout}


{% include links.md %}
