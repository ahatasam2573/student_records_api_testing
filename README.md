# Student Records A Complete Api Testing Project with Postman & Newman
# Endpoints and what i have done in this project

## Base_Url: https://thetestingworldapi.com 

## Get Student 
METHOD: GET 
STATUS CODE: 200 
Request URL: baseUrl/api/studentsDetails 
Response: [ 
{ 
"id": 526717, 
"first_name": "Anna", 
"middle_name": "Banana", 
"last_name": null, 
"date_of_birth":"12/23/1990" 
},
{ 
"id": 526716, 
"first_name": "sample ", 
"middle_name": "sample ", 
"last_name": "sample ", 
"date_of_birth": "sample " 
},
{ 
"id": 526715, 
"first_name": "Anna", 
"middle_name": "Banana last_name=Uzumaki", 
"last_name": null, 
"date_of_birth": "12/23/1990" 
} 
] 

## Create Student 
METHOD: POST 
STATUS CODE: 201 
Request URL: baseUrl/api/studentsDetails 
Body 
{ 
"first_name": "sample string 2", 
"middle_name": "sample string 3", 
"last_name": "sample string 4", 
"date_of_birth": "sample string 5" 
}
Response: { 
"id": 526718, 
"first_name": "sample string 2", 
"middle_name": "sample string 3", 
"last_name": "sample string 4", 
"date_of_birth": "sample string 5" 
} 

### Get Specific Student 
METHOD: GET 
STATUS CODE: 200 
Request URL: baseUrl/api/studentsDetails/id 
Response : { 
"status": "true", 
"data": { 
"id": 526716, 
"first_name": "sample ", 
"middle_name": "sample ", 
"last_name": "sample ", 
"date_of_birth": "sample " 
} 
} 

## Create Technical Skills 
METHOD: POST 
STATUS CODE: 200 
Request Url: 
baseUrl/api/technicalskills 
Body 
{ 
"id": 1, 
"language": [ 
"sample string 1", 
"sample string 2" 
], 
"yearexp": "sample string 2", 
"lastused": "sample string 3", 
"st_id": id 
} 
Response: { 
"status": "true", 
"msg": "Add data success" 
}


### Create Student Address 
METHOD: POST 
STATUS CODE: 200 
Request URL: baseUrl/api/addresses 
Body 
{ 
"Permanent_Address": { 
"House_Number": "sample string 1",
"City": "sample string 2",
 "State": "sample string 3", 
"Country": "sample string 4",
"PhoneNumber": [ 
{ 
"Std_Code": "sample string 1",
"Home": "sample string 2",
 "Mobile": "sample string 3" 
},
{ 
"Std_Code": "sample string 1",
"Home": "sample string 2", 
"Mobile": "sample string 3" 
} 
] 
},
"stId": id 
} 
Response: { 
"status": "true", 
"msg": "Add data success" 
} 

## FINAL STUDENT DETAILS 
METHOD: GET 
STATUS CODE: 200 
Request URL: baseUrl/api/FinalStudentDetails/id 
Response: 
{ 
"status": "true", 
"data": { 
"first_name": "test", 
"middle_name": "123", 
"last_name": "sample string 4", "date_of_birth": "sample string 5", "TechnicalDetails": [ 
{ 
"id": 89801, 
"language": [
"sample string 1", 
"sample string 2" 
], 
"yearexp": "sample string 2", 
"lastused": "sample string 3", 
"st_id": "4165425" 
} 
], 
"Address": [ 
{ 
"Permanent_Address": { 
"House_Number": "sample string 1", 
"City": "sample string 2", 
"State": "sample string 3", 
"Country": "sample string 4", 
"PhoneNumber": [ 
{ 
"Std_Code": "101020", 
"Home": "Dhaka", 
"Mobile": "123456789" 
}, 
{ 
"Std_Code": "sample string 1", 
"Home": "sample string 2", 
"Mobile": "sample string 3" 
} 
] 
}, 
"Current_Address": null, 
"stId": "4165425" 
} 
] 
} 
}

# TEST REPORT

| Name        | Total   | Failed 
| ----------- | ------- | ----- | -------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Iterations`  | 1  | 0 
| `Requests`   | 6 | 0                  |
| `Prerequest Scripts` | 4 | 0
| `Test Scripts` | 6 | 0
| `Assertions` | 23 | 0

Total run duration - 1486ms
Total data received - 11.75KB (approx)
Average response time - 152ms

# Check the Link for better understand of the project
'https://github.com/ahatasam2573/student_records_api_testing/blob/main/newman/Ahatasamul-2023-09-04-11-50-23-403-0.html'