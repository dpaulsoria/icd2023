# How to use Anaconda in console
## Using the console
### Create a new Environment
You can create a new Conda's env using  
`conda create --name envname python=3.8`  
You can activate the env  
`conda activate envname`  
### Install packages
To install packages in your active env
`conda install numpy matplotlib`  
### List your environment
`conda env list`  
### Deactivate your environment
`conda deactivate`  
### Delete your environment  
`conda env remove --name envname`  
## Using YAML
### Create your environment archive
```
name: envname
dependencies:
    - python=3.9
    - numpy
    - matplotlib
```
Then you need to use this command  
`conda env create -f filename.yml`
### Share your current environment
`conda env export > filename.yml`

Currently using 3.11.5