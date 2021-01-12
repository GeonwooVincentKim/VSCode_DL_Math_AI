# VSCode_DL_Math_AI
This is the basic AI-program and codes based on Python with VS-Code.

# Solution of Solving Jupyter-Notebook and Jupyter-Lab Login(Authentication) Problem.
1. Open the Anaconda Navigator (Jupyter Notebook)
2. Open the Anaconda Prompt, and then set to your Virtual-Environment that you gonna use. (conda activate yourVirtualEnviroment)
3. Type 'jupyter notebook --generate-config'
4. Type 'ipython'
5. Type this (This part is register your password)
  - 1. from IPython.lib import passwd
  - 2. passwd()
  - 3. Enter password: 12345 (or 1234)
  - 4. Verify password: 12345 (or 1234)
       (Out[2]: 'sha1:yourToken')
6. Press 'Ctrl+D'(^D), and then press 'y'.

7. Type 'ipython'
8. Type this (This part is authenticate your password)
  - 1. from notebook.auth import passwd;
  - 2. passwd()
  - 3. Enter password: 12345 (or 1234)
  - 4. Verify password: 12345 (or 1234)
       (Out[1]: 'sha1:yourToken')
9. jupyter notebook --NotebookApp.password='sha1:yourToken'
10. Input your password (12345 or 1234) to the 'password [  ] [Log IN]' Section.
