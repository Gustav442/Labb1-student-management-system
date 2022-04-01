# Labb1-student-management-system

POST: localhost:8080/student-management-system/api/students/create
Skapar en student
inga mellanslag/nummer/tecken på firstname och lastname.
email måste ha @ och . och inga mellanslag

Json format : 
{
	"firstName": "Peter",
	"lastName": "Petersson",
	"email": "Peter@gmail.com",
	"phoneNumber": "0707234123"
}

GET: localhost:8080/student-management-system/api/students/"id"
hämtar en student med det id du angett.

GET: localhost:8080/student-management-system/api/students/
hämtar alla students som finns.


GET: localhost:8080/student-management-system/api/students/getlastname?lastName="last name"
hämtar alla vid namn av det efternamn du angett.


DELETE: localhost:8080/student-management-system/api/students/"id"
Tar bort student med det id du angett.


PATCH: localhost:8080/student-management-system/api/students/update/"id"?firstname="new first name"
Byter namn till det namn du angett, på den studenten med det id du angett.


PATCH: localhost:8080/student-management-system/api/students/update/email/"id"
Byter email med json format på den student med det id du angett.

Json format : 
{
	"email": "Berit@gmail.com"
}

