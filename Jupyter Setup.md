### Create Conda Env.
``` bash
conda create -n xeus-cling 
```

### Activate the conda env.
```bash
source activate xeus-cling 
```
### If Jupyter is not installed
<i> If the notebook is installed using pip3, xeus cling won't get detected. </i>

### Installing Jupyter Notebook for xeus cling detection
``` bash
conda install -c conda-forge jupyterlab
conda install -c conda-forge nb_conda_kernels
```

<i>It can happen that jinja2 version is incomaptible, to handle it - </i>
```bash
conda install -c anaconda jinja2
```

<i>To install the extensions </i>
```bash
conda install -c conda-forge jupyter_contrib_nbextensions
```

<b> For C++ 17 Support -  </b>
``` bash
conda install xeus-cling==0.10.0 -c conda-forge
``` 

Enabling nbextension 
``` bash
jupyter nbextension enable varInspector/main
``` 


[References](https://learnopencv.com/xeus-cling-run-c-code-in-jupyter-notebook/)