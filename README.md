# Database Application Setup

This guide provides the necessary steps to install, set up, and run the database application. Follow the instructions below to install dependencies, create and manage the database, and launch the application.

## Prerequisites

1. **SQLite3**  
    Ensure SQLite3 is installed on your system. If not, install it by running:
    ```bash
    sudo apt install sqlite3
    ```
2. Jupyterlab
    Install JupyterLab to run the application’s `.ipynb` notebook:
    ```bash
    pip install jupyterlab
    ```
## Database Setup
### Create the Database
To create the database and populate it with data from `smallRelationsInsertFile.sql`, execute:
```bash
bash createDB.sh
```
### Recreate the Database
To drop all existing tables and reload data from `smallRelationsInsertFile.sql`, run:
```bash
bash recreateDB.sh
```
## Running the Application

1. **Install JupyterLab**  
    If not already installed, run:
    ```bash
    pip install jupyterlab
    ```

2. **Open JupyterLab**  
    Start JupyterLab by running:
    ```bash
    jupyter lab
    ```

3. **Run the Notebook**  
    Open the provided `.ipynb` notebook in JupyterLab and run all the cells to start the application.

4. **Interact with the Database**  
    To interact with the database using the SQLite3 command-line interface, run:
    ```bash
    sqlite3 database/university.db
    ```
    from project root directory, to exit from sqlite3 cli use `Ctrl+D`.