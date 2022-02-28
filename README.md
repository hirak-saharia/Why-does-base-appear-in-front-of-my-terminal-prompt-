# Why-does-base-appear-in-front-of-my-terminal-prompt-

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



  
  
  
