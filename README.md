surfaceProcessing
=================

Package with scripts for running surface level comparison of morphometry

##Installation
download a copy of the repository (or clone it). If the files are packed in a  
zip file (i.e. if you haven't cloned the repo), unpack them using tar -xzfv.  
Then, add the following line to the end of your .bashrc file  

    export PYTHONPATH=/Path/To/The/Downloaded/Files
    
While replacing '/Path/To/The/Downloaded/Files' with the actual absolute  
path that you downloaded the files to

In addition to the files in this repository, please also download the files  
in https://github.com/NeuroanatomyAndConnectivity/glyphsets  
From there, choose whichever runGradientFor###.sh file is appropriate for  
your usage scenario and add put the absolute path to it in the configure.py  
file.


##Usage
Start using the scripts by executing

    python wrapper.py
    
and reading the help file. An example subject list is located at  
/scr/kansas1/surchs/testSurface/subjects.txt and this path is also ideal for  
testing.

If you would like to generate your own subject list, the nifti files are  
located here:

    /scr/melisse1/NKI_enhanced/results/


This is a list of the score options currently implemented for the surface processing  
'pearsonr': pearson correlation between gradient and overlay  
'spearmanr': spearman correlation between gradient and overlay  
'zpear': z-score of correlation p-value of pearson correlation  
'zspear': z-score of correlation p-value of spearman correlation  
