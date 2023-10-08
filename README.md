# Smart-Attendance-System
Smart Attendance System based on Face Recognition using Python and OpenCv.

[**Project Definition**] : Smart Attendance System

[**Problem Statement**] :

The challenge is to develop a Smart Attendance System that utilizes facial recognition technology to automate attendance tracking. Participants will need to create a system that registers and recognizes users' faces, continuously improves its recognition capabilities, logs attendance data into a Firebase database, and generates various reports using a Language Model (LLM) for data analysis. Additionally, a chat interface should be included for database Interaction.

[**Project Description**] :

1. Face Registration and Training:

-As a user, the system allows you to register your face using your laptop or phone camera. Initially, the system captures 10 to 12 images of your face to train its Machine Learning (ML) model. Subsequent       scans for attendance also contribute to the ongoing training of the ML model, making it progressively more accurate with each scan.

2. Realistic Camera Simulation:

-The system should mimic the real-world scenario of two cameras installed at a door,capturing individuals entering or exiting. -The ML model must accurately detect faces in this simulated environment, even when
multiple people are present.

3. Group Attendance Tracking:

-The system should be capable of identifying and logging the attendance of all members in a group.

-When a group enters or exits, the system records all of their entries with timestamps in the Firebase database.

4. Firebase Integration:

-A Firebase database is used to store attendance data securely.

-The system should interact with Firebase to store and retrieve attendance records.

5. Language Model and Chat Interface:

-An LLM is attached directly to the Firebase database for data analysis. -A chat interface allows users to interact with the database for queries and reports.

You need to generate 500 Employees, synthetic data generation and then prepare the reports based on below criteria's :

6. Attendance Reports: -Participants are required to implement various reports using the LLM and database data.

 **These reports Include**:

á. [**Attendance Summary Report**] :- An overview of attendance for all employees, including total hours worked, days present, and days absent.

b. [**Individual Employee Attendance Report**] :- Attendance reports for each employee individually, including daily attendance records and total hours worked.

c. [**Monthly Attendance Report**] :- Summarize attendance data on a monthly basis, displaying attendance patterns by month for all employees.

d. [**Absenteeism Analysis**] :- Identify employees with high absenteeism rates and create a bar chart ranking employees by absenteeism frequency.

e. [**Overtime Report**] :- Calculate overtime hours worked by employees and visualize as a bar chart showing overtime distribution.

f. [**Late Arrival Report**] :- Identify employees with a frequent history of arriving late and create a bar chart showing late arrivals by employee.

g. [**Attendance Trends Over a Year**] :- Analyse attendance trends for all employees over the past year and create a line graph to highlight seasonal variations. 

h. [**Weekly Work Hours Report**] :- Calculate and display weekly work hours for each employee, including a bar chart to show variations in weekly hours worked. 1. Attendance Heatmap: Generate a heatmap to 
   visualize attendance patterns by day and time, identifying peak attendance hours and days.

j. [**Annual Leave Forecast**] :- Predict future leave requests based on historical data and present the forecast as a line chart.

k. [**Quarterly Attendance Trends**] :- Break down attendance trends by quarter and create a line chart to track changes over the year.

1. [**Custom Reports**] :- Allow users to specify criteria for reports (e.g., date range, specific employees) and provide options to export reports in various formats (Excel, PDF).

### Code Requirements
- Opencv(`pip install opencv-python`)
- Tkinter(Available in python)
- PIL (`pip install Pillow`)
- Pandas(`pip install pandas`)

### What steps you have to follow??
- Download my Repository 
- Create a `TrainingImage` folder in a project.
- Open a `AMS_Run.py` and change the all paths with your system path
- Run `AMS_Run.py`.

### Project Structure

- After run you need to give your face data to system so enter your enrollment number and name in box than click on `Take Images` button.
- It will collect 200 images of your faces, it save a images in `TrainingImage` folder
- After that we need to train a model(for train a model click on `Train Image` button).
- It will take 5-10 minutes for training(for 10 person data).
- After training click on `Automatic Attendance` ,it can fill attendance by your face using our trained model (model will save in `TrainingImageLabel` )
- it will create `.csv` file of attendance according to time & subject.
- You can store data in database (install wampserver),change the DB name according to your in `AMS_Run.py`.
- `Manually Fill Attendance` Button in UI is for fill a manually attendance (without facce recognition),it's also create a `.csv` and store in a database.


### Notes
- It will require high processing power(I have 8 GB RAM)
- Noisy image can reduce the accuracy, so quality of images should be good.

### Team Members
- Bhavya Barai
- Kirtan Manek
- Yashkant Prasad
- Darsh Bhoraniya
- Kamalesh Ratanpara
