# bookmarks

pip install -r requirement.txt</br>
python manage.py migrate</br>
python manage.py createsuperuser</br>
python manage.py runserver_plus --cert-file cert.crt</br>

error : there is 1 other session using the database. postgres admin 4 </br>
SELECT *</br>
FROM pg_stat_activity</br>
WHERE datname = 'BookMarks';</br>

sudo service postgresql restart

sudo kill -15 4712 </br>

https://www.postgresqltutorial.com/postgresql-drop-database/

ps -ef | grep postgres
sudo kill -9 9159
