
    Steps for Setting Up Virtual Environment on Ubunbu and Install Common Python Libraries in One Line 
    
### Having troubles to install popular python libraries ? 
### Too time-consuming to install them separately?

 I recently found a way to install "Jupyter notebook, matplotlib, numpy,scipy,scikit-learn,tensorflow" on one command line.
 And it works on Linux , Windows 10 and Virtual environment too.

1. Create Virtual Environment:
(1) pip3 install virtualenv

(2) virtualenv my_working_environment3  (my_working_environment3 is my virtual environment name)

(3) source my_working_environment3/bin/activate  (command to open my virtual environment on Linux or Mac.)
    On windows it would be : activate my_working_environment3 

ps: To remove the virtual environment : rm -rf venv


2. Install python3 and pip3
(1) sudo apt-get install python3
(2) sudo apt autoremove ( optional. Only when step 4 shows " Use 'sudo apt autoremove' to remove them. " ) 
(3) sudo apt-get update  # update first 
(4) sudo apt-get -y install python3-pip
    (If it does not work, use curl "https://bootstrap.pypa.io/get-pip.py" -o "get-pip.py" )



3. Here is the magic code:
   pip3 install --upgrade  numpy pandas scipy scikit-learn jupyter matplotlib tensorflow keras langdetect 
   
   
   
4. Check if the libraries have been successfully installed 
   eg: 
   (1) after "~$ " type : python
   (2) after " >>>" type: from langdetect import detect


ps: It is not recommended to mix different versions of python. Create 2 different virtual environments for 2 versions is a wiser choice.


### Addition notes:
* When I run my codes , it shows "Illegal instruction (core dumped)" after running import tensorflow.
* It happens because your computer CPU requires an earlier tensorflow version . So degrade your version . 

(1) uninstall your tensorflow first by command 
    pip3 uninstall tensorflow 

(2) install tensorflow with earlier version by command 
    pip3 install tensorflow==1.5.0
 
* if error like this occurs in step 2 "Cannot uninstall 'html5lib'. It is a distutils installed project and thus we cannot accurately...." 
*  then install html5lib package before you install the earlier version.
  
* install html5lib by command :  conda install -c anaconda html5lib 
    
Hope it helps!
