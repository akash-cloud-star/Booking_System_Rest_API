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
- Create Data Sets Using the Dynamic Random Variables.
### 2.Verify Created Booking Details
#### In the test case you must be need to validate the following field values:
- First Name
- Last Name
- totalprice
- depositpaid
- bookingdates
- checkin
- checkout
- additionalneeds
### 3.Create Token
Body:
```json
{
	"username": "admin",
	"password": "password123"
}
```
### 4.Verify Updated Student Details
#### In the test case you must be need to validate the following field values:
- First Name
- Middle Name
- Last Name
- Date of Birth
### 5.Create Technical skills Create Student Address
#### In the test case you must be need to validate the following field values:
- Only Message
### 6.Get the Student's Full Details
#### In the test case you must be need to validate the following field values:
- First Name
- Middle Name
- Last Name
- Date of Birth
- Language
- Year Of Experience
- Last Used Date
- City
- House Number
- Country
- State
- Home Address
- Std Code
- Mobile
### 7.Delete Specific Student
#### In the test case you must be need to validate the following field values:
- Only Message
# Newman Report

![Screenshot 2023-05-29 194425](https://github.com/akash-cloud-star/Student_Rest_API/assets/61002722/332962d3-8291-4eaf-8385-49a1800c66b8)
![Screenshot 2023-05-29 194439](https://github.com/akash-cloud-star/Student_Rest_API/assets/61002722/2eca098d-0f53-4f75-810a-f99381cc61ac)
![Screenshot 2023-05-29 194453](https://github.com/akash-cloud-star/Student_Rest_API/assets/61002722/c0eafaf7-5bcf-43aa-abcd-81be02cc9858)


