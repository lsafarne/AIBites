
Overview


```python
%pip install nbconvert
```

    Requirement already satisfied: nbconvert in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (6.0.7)
    Requirement already satisfied: nbformat>=4.4 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (5.1.2)
    Requirement already satisfied: traitlets>=4.2 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (5.0.5)
    Requirement already satisfied: entrypoints>=0.2.2 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (0.3)
    Requirement already satisfied: mistune<2,>=0.8.1 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (0.8.4)
    Requirement already satisfied: testpath in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (0.4.4)
    Requirement already satisfied: jupyter-core in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (4.7.0)
    Requirement already satisfied: pandocfilters>=1.4.1 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (1.4.3)
    Requirement already satisfied: pygments>=2.4.1 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (2.7.4)
    Requirement already satisfied: nbclient<0.6.0,>=0.5.0 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (0.5.1)
    Requirement already satisfied: defusedxml in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (0.6.0)
    Requirement already satisfied: jupyterlab-pygments in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (0.1.2)
    Requirement already satisfied: bleach in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (3.2.2)
    Requirement already satisfied: jinja2>=2.4 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbconvert) (2.11.2)
    Requirement already satisfied: MarkupSafe>=0.23 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from jinja2>=2.4->nbconvert) (1.1.1)
    Requirement already satisfied: jupyter-client>=6.1.5 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbclient<0.6.0,>=0.5.0->nbconvert) (6.1.11)
    Requirement already satisfied: async-generator in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbclient<0.6.0,>=0.5.0->nbconvert) (1.10)
    Requirement already satisfied: nest-asyncio in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbclient<0.6.0,>=0.5.0->nbconvert) (1.4.3)
    Requirement already satisfied: ipython-genutils in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbformat>=4.4->nbconvert) (0.2.0)
    Requirement already satisfied: jsonschema!=2.5.0,>=2.4 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from nbformat>=4.4->nbconvert) (3.2.0)
    Requirement already satisfied: webencodings in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from bleach->nbconvert) (0.5.1)
    Requirement already satisfied: six>=1.9.0 in /Users/lidasafarnejad/Library/Python/3.7/lib/python/site-packages (from bleach->nbconvert) (1.15.0)
    Requirement already satisfied: packaging in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from bleach->nbconvert) (20.8)
    Requirement already satisfied: pyrsistent>=0.14.0 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat>=4.4->nbconvert) (0.17.3)
    Requirement already satisfied: importlib-metadata in /Users/lidasafarnejad/Library/Python/3.7/lib/python/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat>=4.4->nbconvert) (3.3.0)
    Requirement already satisfied: attrs>=17.4.0 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat>=4.4->nbconvert) (20.3.0)
    Requirement already satisfied: setuptools in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from jsonschema!=2.5.0,>=2.4->nbformat>=4.4->nbconvert) (39.0.1)
    Requirement already satisfied: pyzmq>=13 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from jupyter-client>=6.1.5->nbclient<0.6.0,>=0.5.0->nbconvert) (21.0.1)
    Requirement already satisfied: tornado>=4.1 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from jupyter-client>=6.1.5->nbclient<0.6.0,>=0.5.0->nbconvert) (6.1)
    Requirement already satisfied: python-dateutil>=2.1 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from jupyter-client>=6.1.5->nbclient<0.6.0,>=0.5.0->nbconvert) (2.8.1)
    Requirement already satisfied: pyparsing>=2.0.2 in /Library/Frameworks/Python.framework/Versions/3.7/lib/python3.7/site-packages (from packaging->bleach->nbconvert) (2.4.7)
    Requirement already satisfied: typing-extensions>=3.6.4 in /Users/lidasafarnejad/Library/Python/3.7/lib/python/site-packages (from importlib-metadata->jsonschema!=2.5.0,>=2.4->nbformat>=4.4->nbconvert) (3.7.4.3)
    Requirement already satisfied: zipp>=0.5 in /Users/lidasafarnejad/Library/Python/3.7/lib/python/site-packages (from importlib-metadata->jsonschema!=2.5.0,>=2.4->nbformat>=4.4->nbconvert) (3.4.0)
    
    [1m[[0m[34;49mnotice[0m[1;39;49m][0m[39;49m A new release of pip available: [0m[31;49m22.3.1[0m[39;49m -> [0m[32;49m23.2.1[0m
    [1m[[0m[34;49mnotice[0m[1;39;49m][0m[39;49m To update, run: [0m[32;49m/Library/Frameworks/Python.framework/Versions/3.7/bin/python3.7 -m pip install --upgrade pip[0m
    Note: you may need to restart the kernel to use updated packages.



```python
%jupyter nbconvert --to markdown  notebook.ipynb
```
