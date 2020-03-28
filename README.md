# Pipenv Understanding
## Day 1

- `pipenv install` to create workspace and install dependencies
- `pipenv shell` to activate the virtual env
- Once the shell is activated, run `python hello.py` to bring the Flask App UP!!
- By default the flash app runs on port 5000 - `http://localhost:5000/hello`
- `pipenv install fpdf` - install the fpdf module which is used to create the pdf
- Acticate the shell again to execute `python pdf_create.py` which will create `example.pdf`
- `pipenv install PyPDF2` - install the PyPDF2 module which is used to read the pdf content
- Acticate the shell again to execute `python pdf_Reader.py` which will read the contents of `example.pdf`
- `basics.py` contains all the basic syntaxes in python
- `modules.py` 
        - python searches the list of directories from `sys.path`. Use `sys.path.append(directory_path)` to add directory searches during import.

  ```python
    python3
    >>> import sys
    >>> sys.path
    ['', '/usr/local/Cellar/python/3.7.5/Frameworks/Python.framework/Versions/3.7/lib/python37.zip', '/usr/local/Cellar/python/3.7.5/Frameworks/Python.framework/Versions/3.7/lib/python3.7', '/usr/local/Cellar/python/3.7.5/Frameworks/Python.framework/Versions/3.7/lib/python3.7/lib-dynload', '/usr/local/lib/python3.7/site-packages']
  ```

  - Alternatively use `PYTHONPATH` to set the package/module import paths.
    - If a package has `__init__.py`, it becomes a module
    - `learn` is a module which is used in `modules.py`