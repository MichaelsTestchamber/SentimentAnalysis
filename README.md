# SentimentAnalysis
---
## Managing virtual enviroment:
---
### Conda commands:
> Use base enviroment: ```conda activate base```

> Deactivate enviroment: ```conda deactivate```

> List enviroment: ```conda env list```

> Create enviroment: ```conda create -n <my_env_name>```
- > With version control: ```conda create -n <my_env_name>  python=3.6```
- > With instruction file: ```conda env create -f environment.yml```

> Delete enviroment: ```conda env remove -n <my_env_name>```
---
### Pip commands:
> Install kernel: ```pip install --user ipykernel```

> Install requirements file: ```pip install -r /path/to/requirements.txt```

> Write requirements file: ```pip freeze > requirements.txt```
---
### Python commands:
> Add kernel to enviroment> ```python -m ipykernel install --user --name=<my_env_name>```
---
### Jupyter commands:
> List kernels: ```jupyter kernelspec list```

> Remove kernel: ```jupyter kernelspec remove <my_env_name>```
---
## YML Example
---
### YML Overview:
File extension: ```.yml```

Code:

```
name: <my_env_name>

dependencies:
- python=3.6
- pip:
  - mxnet==1.5.0
  - d2lzh==0.8.11
  - jupyter==1.0.0
  - matplotlib==2.2.2
  - pandas==0.23.4
  ```