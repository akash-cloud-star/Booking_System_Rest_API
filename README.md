# [Booking_System_Rest_API]
## :page_facing_up: API Test Report
## :memo: How to run this project
### 🖥 Run by Postman
* Clone this repository.
* Import collection and environment file/link.
* Run the collection on Postman.
### 🖥 Run by Newman
* Clone this repository.
* Open cmd to the file location.
* Run Command:
console
newman run First.postman_collection.json -e Batchit.postman_environment.json
* Run Command for Report:

For html:
console
newman run First.postman_collection.json -e Batchit.postman_environment.json -r cli,html
For htmlextra:
console
newman run First.postman_collection.json -e Batchit.postman_environment.json -r cli,htmlextra
### :technologist: Technology used
<img src="https://voyager.postman.com/logo/postman-logo-icon-orange.svg"  width="15" height="15"> Postman & Newman
### Prerequisite
- Jdk
- Node Js
- Newman
- Html Report Library

### Newman and Report Installation Process
- Newman Install Command:
 console
npm install -g newman-reporter-htmlextra
- Newman Html Report Install Command:
 console
npm install -g newman-reporter-htmlextra
### API Documentations
[PDF](https://docs.google.com/document/d/1YyzPMbEu6eEMFrvp-WHiJW-SvDTJvikqx1QGyyFgRXw/edit?usp=sharing)
#### Postman Documentations
[Postman](https://documenter.getpostman.com/view/25930416/2s93mAUfPS)
## Test case list:
### 1.Create Booking System

### 2.Verify Created Booking Details
``` url
https://restful-booker.herokuapp.com/booking/
```
```json
  https://restful-booker.herokuapp.com/booking \
  -H 'Content-Type: application/json' \
  -d '{
	"firstname" : "Jim",
	"lastname" : "Brown",
	"totalprice" : 111,
	"depositpaid" : true,
	"bookingdates" : {
    	"checkin" : "2018-01-01",
    	"checkout" : "2019-01-01"
	},
	"additionalneeds" : "Breakfast"
}'

```

#### In the test case you must be need to validate the following field values:
Body :
```json
{
	"firstname": "Sally",
	"lastname": "Brown",
	"totalprice": 111,
	"depositpaid": true,
	"bookingdates": {
    	"checkin": "2013-02-23",
    	"checkout": "2014-10-23"
	},
	"additionalneeds": "Breakfast"
}

```
### 3.Create Token
``` url
https://restful-booker.herokuapp.com/auth
```
Body :
```json
{
	"username": "admin",
	"password": "password123"
}
```
### 4.Verify Updated Booking Details
``` url
https://restful-booker.herokuapp.com/booking/id
```
```json


  -H 'Cookie: token=abc123' \
  -d '{
	"firstname" : "James",
	"lastname" : "Brown",
	"totalprice" : 111,
	"depositpaid" : true,
	"bookingdates" : {
    	"checkin" : "2018-01-01",
    	"checkout" : "2019-01-01"
	},
	"additionalneeds" : "Breakfast"
}

```
### 7.Delete Specific Student
#### In the test case you must be need to validate the following field values:
``` url
https://restful-booker.herokuapp.com/booking/1
```
# Newman Report

![Screenshot 2023-05-31 171318](https://github.com/akash-cloud-star/Booking_System_Rest_API/assets/61002722/91d39135-a620-427f-9827-682678216fba)
![Screenshot 2023-05-31 171342](https://github.com/akash-cloud-star/Booking_System_Rest_API/assets/61002722/8def37fa-34ed-4323-985d-e0be6ec3437b)
![Screenshot 2023-05-31 171406](https://github.com/akash-cloud-star/Booking_System_Rest_API/assets/61002722/c21a7d2e-aaee-409f-a4dd-e39efda68912)



