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

![Screenshot (1)](https://user-images.githubusercontent.com/107624668/210522229-07245450-4634-46b0-ae60-a2c00a46860c.png)

2.Use this **http://localhost:5000/api/v1/doctors/login** to login as a doctor and add info as shown in image

![Screenshot (2)](https://user-images.githubusercontent.com/107624668/210522400-c2c6c906-16a5-4757-9e53-b77837f8c6f7.png)

3.Use this **http://localhost:5000/api/v1/patients/register** and add the token in authorization area which is recieved in second point

![Screenshot (3)](https://user-images.githubusercontent.com/107624668/210522471-173a8b1b-c039-4167-9224-fdef51485a5f.png)

4. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/create_report** to create report and add status you can see the types of 
   status in report model.

![Screenshot (4)](https://user-images.githubusercontent.com/107624668/210522551-9703587d-d232-4788-99bd-4a023b1f7802.png)

5. Use this **http://localhost:5000/api/v1/patients/62c31cc86a84003324d04cb5/all_reports** to get all the reports.

![Screenshot (5)](https://user-images.githubusercontent.com/107624668/210522595-06a98f9f-3b14-4abc-bae5-2d8dc79d7600.png)

# DEPLOYEMENT
Project already deployed on render(For better exp: use Postman for accesing above Routes)

Do Visit: https://hospital-api-prem.onrender.com/api/v1/doctors/register
