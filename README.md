# Inititalizing Conda Environemnts in Jupyter

Basic outline to initialize environments with R or Python kernels in Jupyter platforms

### R

Create and activate the environment  
`conda create -n r-kernel`  
`conda activate r-kernel`

Install the R-kernel and Jupyter packages  
`conda install r-recommended r-irkernel`  
`conda install Jupyter`  

Add the R-kernel to Jupyter  
`R -e 'IRkernel::installspec()'`  

### Python

Type `bash` in the terminal to make sure you are using a bash terminal.  
Type `conda init` to make sure conda is activated.  
To create a new environment "env_name" type `conda create -n <env_name>`.  
To activate the new environment "env_name" type conda `activate <env_name>`.  
To install packages type `conda` or `pip` + `install <pkg_name>==<ver>`.  
To link the new environment to JupyterHub type `conda install -c anaconda ipykernel` and then type `ipython kernel install --user --name=<env_name>`.  
