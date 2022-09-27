# Setting up Python workspace

----------

1. Install Python from <https://www.python.org/downloads/>

2. Install Pip - Note: This is usually included in the latest release of Python 3.x or 2.x but if you need to install manually go to this link :<https://pip.pypa.io/en/stable/installing/>

```console
Useful pip commands

pip --help

pip list

pip install <package name>

pip uninstall <package name>

pip show - This will show you the package information and 
dependencies or requirements
```

**NOTE:** Never ever install third-party packages outside virtualenv. Remember to always use/activate virtualenv before installing anything using pip

1. Install virtualenv using pip:
```console 
python -m pip install virtualenv

python3 -m pip install virtualenv
```

2. To use virtualenv, 
```console
a. create a directory that will hold your projects/scripts
	mkdir virtualenvs

	cd virtualenvs

b. Create virtualenv
	virtualenv -p python3/python <project name>

	cd <project name>\scripts\

	.\activate

c. to Deactivate 
	deactivate
```

3. Start installing packages or libraries
```console
	a. Recommended libraries to install to any kind of projects
		python -m pip install pylint, pycodestyle, black, ipython
```

4. To create requirements.txt file, so that all the members of the project have an identical environment run the command
```console
	python -m pip freeze > requirements.txt 
	
	Note: this will list all the dependency libraries you used on your project and save it to txt file.
```

5. To install the requirements.txt
```console
	python -m pip install -r requirements.txt
```
