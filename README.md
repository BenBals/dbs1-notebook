# Installation and First Startup

The notebook is based on the SQLite3 kernel for jupyter nootebook, a lightweight DBMS. To use it, you must have python3 installed.

Open a terminal in the notebooks directory and follow the steps below:

0) Make sure you have SQLite installed (usually called `sqlite3`):
    e.g. on OSX
    ```console
    brew install sqlite3
    ```
    or on Ubuntu
    ```console
    sudo apt-get install sqlite3
    ```

1) Create a virtual environment for this notebook:

	```console
	python3 -m venv venv
	```

2) Activate the virtual environment on unix machines:

	```console
	source venv/bin/activate
	```

	Or on Windows:

	```console
	.\venv\Scripts\activate
	```

3) Install the dependencies of this notebook:

	```console
	pip install -r requirements.txt
	```

4) Clone the repository of the sqlite3-kernel:

	```console
	git clone https://github.com/brownan/sqlite3-kernel.git
    ```

5) Change the directory and install the sqlite3-kernel:

 	```console
    cd sqlite3-kernel
    python setup.py install
    python -m sqlite3_kernel.install
    ```

6) Go back to your notebook directory and start the notebook server:

 	```console
    cd ..
	jupyter notebook
    ```

7) Now a tab will open in your browser. If you click on `Interactive_sql.ipynb` from the displayed files, the notebook will open. Remember that you should not close the terminal as long as you want to work with the notebook.

# Normal Startup

If you want to start the notebook and have already done the installation, you only have to execute the following two commands in your notebook directory:

1) Activate the virtual environment on unix machines:

	```console
	source venv/bin/activate
	```

	Or on Windows:

	```console
	.\venv\Scripts\activate
	```

2) Start the notebook server:

	```console
	jupyter notebook
	```
