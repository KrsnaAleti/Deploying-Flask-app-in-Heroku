# Deploying-Flask-app-in-Heroku
https://github.com/KrsnaAleti/My_Resources/tree/main/Flask_Database_Heroku

### This Project covers the following:
* An application created using Flask in Python
* Connecting with Database - sqlite/MySQL
* Deployment in Heroku


## Notes:
1. We can get the code snippets for flask-database usage from the below urls:
   * https://flask.palletsprojects.com/en/2.1.x/quickstart/
   * https://flask-sqlalchemy.palletsprojects.com/en/2.x/quickstart/#a-minimal-application

2. Database configuration - code snippet:- https://flask-sqlalchemy.palletsprojects.com/en/2.x/config/

3. If we get module not found error for mysql db, we can are use pymysql
   * https://stackoverflow.com/questions/454854/no-module-named-mysqldb
   * We need to edit the SQLAlchemy URL schema like this: mysql+pymysql://username:passwd@host/database as we are installed PyMySQL.

4. Defining the class to create the table and defining the columns of the taable:-
   * https://flask-sqlalchemy.palletsprojects.com/en/2.x/quickstart/#a-minimal-application
   * https://flask-sqlalchemy.palletsprojects.com/en/2.x/models/

5. Inserting values in the database:-
   * https://flask-sqlalchemy.palletsprojects.com/en/2.x/queries/?highlight=insert

### List of commands to use for deploying into Heroku:
1. heroku login

2. pip install gunicorn
3. pip freeze requirements.txt
4. Procfile
   * web: gunicorn app:app
5. git init
6. git add
7. git commit -m "Initial commmit"
8. heroku create appname
9. git remote -v
10. git push heroku master

