
**Python 3.4+ and above**
Creating virtual env 
```
python -m venv <folder_name>
```

Activate venv
```
source <folder_name>/bin/activate
```

Deactivate venv
```
deactivate
```

Delete venv
```
deactivate
rm -r <folder_name>
```

Display all the packages installed in the venv
```
pip list
```

Create requirements file from venv
```
pip freeze > requirements.txt
```


Install packages requirements file
```
python -m pip install -r requirements.txt
```
