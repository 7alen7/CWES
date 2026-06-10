# Web Requests Module Notes

### cURL POST format

curl -H 'Content-Type: application/json' -X POST -d '{"search":"flag"}' -b 'PHPSESSID=nmhcmat3eib8jiknuqe45r8kau' http://154.57.164.80:32750/search.php


### CRUD API

Create	POST	Adds the specified data to the database table
Read	GET	Reads the specified entity from the database table
Update	PUT	Updates the data of the specified database table
Delete	DELETE	Removes the specified row from the database table

curl -X POST http://<SERVER_IP>:<PORT>/api.php/city/ -d '{"city_name":"HTB_City", "country_name":"HTB"}' -H 'Content-Type: application/json'

curl -X GET http://<SERVER_IP>:<PORT>/api.php/city/london

curl -X PUT http://<SERVER_IP>:<PORT>/api.php/city/london -d '{"city_name":"New_HTB_City", "country_name":"HTB"}' -H 'Content-Type: application/json'

curl -X DELETE http://<SERVER_IP>:<PORT>/api.php/city/New_HTB_City

