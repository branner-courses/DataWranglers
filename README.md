## Data Wranglers Projects

### Installation of PyTables

Using `pip`, even following many published suggestions, generated errors on Mac OS 10.9.5 with Python 3 (Python 2 also failed). The following worked:

```
brew install hdf5
virtualenv v_env3 --python=python3
. v_env3/bin/activate
pip install ipython numpy scipy matplotlib numexpr
pip install --upgrade git+git://github.com/cython/cython@master

# Downloaded from http://sourceforge.net/projects/pytables/?source=typ_redirect
# cd into directory
# following http://pytables.github.io/usersguide/installation.html
python setup.py build --hdf5=/usr/local/Cellar/HDF5/1.8.13
```

On the need for `hdf5`, see https://www.underworldproject.org/documentation/HDF5Download.html.

[end]
