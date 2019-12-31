References : 
 * https://conda.io/projects/conda/en/latest/user-guide/install/linux.html
 * https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/20/conda/

### This section is for installing conda on your Linux machine
1. Download the installer:  ( I chose this miniconda) 

        Miniconda installer for Linux.  

        Anaconda installer for Linux.

 2. In your terminal window, run: ( here, you must open the terminal in the same directory with this file)

        Miniconda: bash Miniconda3-latest-Linux-x86_64.sh  
        
        Anaconda: bash Anaconda-latest-Linux-x86_64.sh

 3. Follow the prompts on the installer screens.If you are unsure about any setting, accept the defaults by pressing 'Enter'. 
    You can change them later.

 4. To make the changes take effect, close and then re-open your terminal window.

 5. Test your installation, type: conda -V
 
 6. Uninstalling Anaconda or Miniconda

    Open a terminal window and Remove the entire miniconda install directory with:   rm -rf ~/miniconda

### This section is for windows miniconda installation
download the version you need via this link :  https://docs.conda.io/en/latest/miniconda.html

These Miniconda installers contain the conda package manager and Python. Once Miniconda is installed, you can use the conda command to install any other packages and create environments. 

     you must use conda shell prompt ( click window icon at left bottom )
       
     eg: $ conda install numpy
     eg: $ conda create -n myenv 

 
 ### This section is for creating virtual environment and installing libraries for conda on windows 
  
     you must use conda shell prompt ( click window icon at left bottom ) 
  
 1. Update conda by typing : conda update conda
 
 2. Create your virtual environment : conda create -n my_working_environment3 python=3.6 
     
         'my_working_environment3' is my virtual environment name (choose a name for yourself ) 
          Python version is specified to 3.6 (optional) 
          you can change to your reference. This step may take a while depends on your machine. 
 
 3. Activate your virtual environment : conda activate my_working_environment3  
 
         (Again, my_working_environment3' is my virtual environment name. You can change to yours )
 
 4. Install python libraries in the virtual environment:  ( you can install all libraries in a single line ) 
 
        conda install -n my_working_environment3 numpy pandas scipy scikit-learn jupyter matplotlib tensorflow keras 
    
 5. Check the libraries installed : conda list
 
 You are all set  !!!!!
 
 6. Deactiavte your virtual environment:  source deactivate ( if it does not work, try type : 'conda deactivate')
 
 7. Delete a virtual environment : conda remove -n yourenvname -all
 
