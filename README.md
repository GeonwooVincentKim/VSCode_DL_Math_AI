# VSCode_DL_Math_AI
This is the basic AI-program and codes based on Python with VS-Code.

# Solution of Solving Jupyter-Notebook and Jupyter-Lab Login(Authentication) Problem.
  - I. Open the Anaconda Navigator (Jupyter Notebook)
  - II. Open the Anaconda Prompt, and then set to your Virtual-Environment that you gonna use. (conda activate yourVirtualEnviroment)
  - III. Type 'jupyter notebook --generate-config'
  - IV. Type 'ipython'
  - V. Type this (This part is register your password)
    -> I. from IPython.lib import passwd
    -> II. passwd()
    -> III. Enter password: 12345 (or 1234)
    -> IV. Verify password: 12345 (or 1234)
         (Out[2]: 'sha1:yourToken')
  - VI. Press 'Ctrl+D'(^D), and then press 'y'.

  - VII. Type 'ipython'
  - VIII. Type this (This part is authenticate your password)
    -> I. from notebook.auth import passwd;
    -> II. passwd()
    -> III. Enter password: 12345 (or 1234)
    -> IV. Verify password: 12345 (or 1234)
         (Out[1]: 'sha1:yourToken')
  - IX. jupyter notebook --NotebookApp.password='sha1:yourToken'
  - X. Input your password (12345 or 1234) to the 'password [  ] [Log IN]' Section.
