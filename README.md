# LADAL Interactive notebooks

[Launch Notebooks](https://mybinder.org/v2/gh/SLCLADAL/interactive-notebooks-environment/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252FSLCLADAL%252Finteractive-notebooks%26urlpath%3Dlab%252Ftree%252Finteractive-notebooks%252F%26branch%3Dmain)

This repository holds a series of interactive notebooks to be run on any Binder instance. Click the link above to launch a live instance with everything you need to run these already installed.


## Contributing

Dependencies are managed in [the environment repository](https://github.com/SLCLADAL/interactive-notebooks-environment), 
to ensure that the slow process of rebuilding and installing all of the R
packages only needs to happen when dependencies change, not on every commit
to this repository.

## Generating a New Notebook Link

Use the [nbgitpuller link generator](https://hub.jupyter.org/nbgitpuller/link.html) to generate links for new notebooks.

The parameters you need are:

BinderHub URL

  - https://mybinder.org OR
  - https://binderhub.atap-binder.cloud.edu.au/

Git *Environment* Repository URL and Branch - note that the base environment is where the dependencies live, the content is copied from the interactive-notebooks environment on top of this.
  
  - https://github.com/SLCLADAL/interactive-notebooks-environment
  - main

Git *Content* Repository URL and Branch

  - https://github.com/SLCLADAL/interactive-notebooks
  - main

File to Open - this is the path in the *content* repository

  - notebooks/<whatever>.ipynb

Application to Open

  - JupyterLab
