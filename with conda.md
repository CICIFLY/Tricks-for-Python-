References : 
 * https://conda.io/projects/conda/en/latest/user-guide/install/linux.html
 * https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/20/conda/

### This section is for installing conda on your Linux machine
1. Download the installer:

        Miniconda installer for Linux.  ( I chose this one) 

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


 
 ### This section is for create virtual environment 
 1. Update conda by typing : conda update conda
 2. Create your virtual environment : conda create -n my_working_environment3 python=3.6 anaconda
    ('my_working_environment3' is my virtual environment name .  Python version is specified to 3.6. you can change to your reference. This step may take a while depends on your machine )
 3. Activate your virtual environment : source activate yourenvname
 4. Install python libraries in the virtual environment:  conda install -n my_working_environment3 numpy pandas scipy scikit-learn jupyter matplotlib tensorflow keras langdetect 
