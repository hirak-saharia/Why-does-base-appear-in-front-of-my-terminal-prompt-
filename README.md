
# Why-does-base-appear-in-front-of-my-terminal-prompt-


To open anaconda-navigator from terminal type : 
   
     source /home/hirak/anaconda3/bin/activate
     
     

Two ways to set activate/Deactivate Base Environment in Ubuntu terminal

1.

This can also be because auto_activate_base is set to True. You can check this using the following command
   
   conda config --show | grep auto_activate_base
   

To set it false

  conda config --set auto_activate_base False
  
  source ~/.bashrc
  

To reactivate set it to True

  conda config --set auto_activate_base True
  
  
  source ~/.bashrc
  


2.  (base) appears due to change in conda environment.

   To deactivate a conda environment, enter:
    
    conda deactivate

  To activate Base for Opening Anaconda-Navigator or Jupyter notebook
    
    conda activate base
    
  Or To revert it back to normal you can run the command:
     
     conda init --reverse



The best and easy way to install anaconda on Ubuntu for GUI Version

The steps are as follows:
  1. Download anaconda from https://www.anaconda.com/
  2. Open the terminal from the folder where anaconda is downloaded
  3. Type: $bash anaconda_file_name.sh
  4. Follow the instructions as stated in the terminal.
  5. Close the terminal and open a new terminal window
  6. If (base) is not shown in terminal:
      a.  Type in terminal $ nano ~.bashrc
      b.  Paste the following in the end of file:
                export PATH="/home/user_name/anaconda3/bin:$PATH"
  7. Open a text editor and save it as anaconda.desktop on the desktop.
  8. Paste the following into the editor

#!/usr/bin/env xdg-open
[Desktop Entry]
Name=Anaconda
Version=2.0
Type=Application
Exec=/home/user_name/anaconda3/bin/anaconda-navigator
Icon=/home/user_name/anaconda3/lib/python3.8/site-packages/anaconda_navigator/static/images/anaconda-icon-256x256.png
Comment=Open Anaconda Navigator
Terminal=false 

  9. Save and close the file.
10. Go to desktop, right click on anaconda.desktop and click on "Allow Launching"


  
  
  
