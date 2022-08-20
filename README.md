# Information about API:
### Theme:
- We’re going to design an API for the doctors of a Hospital which has been allocated by the
govt for testing and quarantine + well being of COVID-19 patients
- There can be 2 types of Users
- Doctors
- Patients
- Doctors can log in
- Each time a patient visits, the doctor will follow 2 steps
- Register the patient in the app (using phone number, if the patient already exists, just
return the patient info in the API)
- After the checkup, create a Report
- Patient Report will have the following fields
- Created by doctor
- Status (You can use enums if you want to):
- Can be either of: [Negative, Travelled-Quarantine, Symptoms-Quarantine,
Positive-Admit]

- Date

# Instructions about SetUp:

First start with downloading the code and and write npm install on code editor, it will install all dependencies on your editor.
You will need a code editor and mongoDB setup on your computer.
We will use postman to check the api is working or not,So download postman on your computer.

1.Now use this **http://localhost:5000/api/v1/doctors/register** route to register doctor in API and add the info as shown in image

![1](https://user-images.githubusercontent.com/101451924/185754068-67021b2a-af59-4fff-9af5-4a783bc46a90.png)


2.Use this **http://localhost:5000/api/v1/doctors/login** to login as a doctor and add info as shown in image

![2](https://user-images.githubusercontent.com/101451924/185754072-595c68a2-1d27-4e9e-b21d-b2f6b44202c6.png)

3.Use this **http://localhost:5000/api/v1/patients/register** and add the token in authorization area which is recieved in second point

![3](https://user-images.githubusercontent.com/101451924/185754077-8e82542a-dfd9-4ff7-b097-4821bdb52e41.png)


4. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/create_report** to create report and add status you can see the types of 
   status in report model.

![4](https://user-images.githubusercontent.com/101451924/185754082-588c13a9-177b-4d16-a527-74dedca6584d.png)


5. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/all_reports** to get all the reports.

![5](https://user-images.githubusercontent.com/101451924/185754089-35b8db22-dfcb-4eee-899c-b3d3a014b365.png)

# DEPLOYEMENT
Project already deployed on Heroku(For better exp: use Postman for accesing above Routes)

Do Visit: https://hospitalapi0.herokuapp.com/api/v1/doctors/register
