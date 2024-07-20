# unblocklife - CMS System Name 

This is based on Wagtail CMS.  The Wagtail comes with several built-in features to support users with accessibility needs and an accessibility checker to encourage accessible content creation. We are also proud Wagtail CMS is a trusted tool used by the Royal National Institute of Blind People.

## Installing this instance

```
git clone git@github.com:dravate/unblocklife.git
cd unblocklife
pipenv --python /usr/bin/python3
pipenv shell
pip install -r requirements.txt 
python manage.py makemigrations home courses 
python manage.py migrate
python manage.py runsever

```

You can access the site at ```http://localhost:8000``` 


Offcourse - After that you need to

```
python manage.py createsuperuser

```
and use admin interface to start modifying/adding content. 

## Demo Data Site 

We have also added ```media``` folder with data & added  backup data as file  ```demo_data.sqlite3```. Just copy and run the server, you can see the instance running with demo data. 

```
cp demo_data.sqlite3 db.sqlite3
python manage.py createsuperuser
python manage.py runsever

```

You can access the site at ```http://localhost:8000``` 







