# python_package
### conda
```python
conda create --name environmentname
source activate environmentname
conda install numpy
```

### pip and venv
```
python3 -m venv environmentname
source environmentname/bin/activate
pip install numpy
```

### PyPi vs. test PyPi
```
cd binomial_package_files
python setup.py sdist
pip install twine

# commands to upload to the pypi test repository
twine upload --repository-url https://test.pypi.org/legacy/ dist/*
pip install --index-url https://test.pypi.org/simple/ dsnd-probability

# command to upload to the pypi repository
twine upload dist/*
pip install dsnd-probability
```
