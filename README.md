## Augur
***
Augur is a webapp for tracking reference desk statistics for libraries, inspired by libstats. It was written in Python and Javascript.   

In Ubuntu:

sudo apt-get install python-pip python-dev build-essential 

sudo pip install --upgrade pip

sudo pip install --upgrade virtualenv

sudo apt-get install git

sudo apt-get install mysql-server

sudo apt-get install python-mysqldb

mysql -u root -p

create database refstatsdb;

git clone https://github.com/Zwounds/refstats.git

pip install -r requirements.txt

python manage.py restart_db

gunicorn -w 4 -u 0.0.0.0:5000 augur:app

Now Augur is running on port 5000. Change the default password in manage.py line 21.
