## 05/15/2023 to 06/04/2023

<span id="topo">

<h1 align="center">:bookmark: Fourth Delivery - SPRINT 4</h1>

<p align="center">
     <a href="#goals">Sprint goals</a> &nbsp |&nbsp &nbsp
     <a href="#deliveries">Deliveries</a> &nbsp |&nbsp &nbsp
     <a href="#burndown">Burndown</a> &nbsp |&nbsp &nbsp
     <a href="#backlogs">Backlogs</a>
</p>

We have the challenge of implementing the limitation of network bandwidth consumption in the system configuration screen, and including graphs in the dashboard for user analysis.

<span id="goals">
    
## :dart: Sprint Goals
The requirements (both customer and educational institution) covered for third sprint are:
- **RF 07:** Network Bandwidth Consumption Limitation
- **RF 17:** Dashboard Improvements (Graphics)
- **RNF 11:** Tests
- **RNF 13:** Scan time (how often the system checks for new files)
    
<br>
 
**:link: Click the link below to view the *Kanban* of team activities:**
> [Kanban Projects GitHub](https://github.com/orgs/TechNinjass/projects/2)
    
<br>     
     
## :closed_book: DevOps

This repository contains the documentation of each DevOps item implemented in the FATEC project with Midall during the 5th semester of the Database course. It provides a detailed description of each item, explaining our DevOps workflow, methodologies used, tools used, technologies chosen, and much more.
 
#### 🔗 [Wiki Documentation Link](https://github.com/TechNinjass/midall-parent/wiki)       
     
<br>     
     
<span id="deliveries">
  
## :heavy_check_mark: Deliveries
    
### :heavy_check_mark: RF 07: Network Bandwidth Consumption Limitation
     
In this sprint, we implemented the option for the user to limit the network bandwidth when transferring the file, through the configuration screen with the requested parameters. In the front-end, the user will define an "x" bandwidth value, if in the transfer process the file exceeds this limit, the system will stop transferring the file.
     
### :heavy_check_mark: RF 17: Dashboard Improvements (Graphics)
  
📊 We made the logic of the "CASE WHEN" where: if the value of the column "Status" is equal to 'transferred', then the value of the new column "New_Status" will be 1. Otherwise, if the value of the column "Status" is different of 'transferred' (that is, any other value), the value of the new column "New_Status" will be 0.

<details>

<summary>Code of Logic Implemented in LookerStudio</summary>     
     
```sql
     
SELECT 
  CASE 
    WHEN Status = 'transferido' THEN 1
    ELSE 0
  END AS New_Status
FROM 
  [dbo].[file_transfer]
     
```
     
</details>
     
By presenting the data in this simplified way on the dashboard, you can get a clearer, easier-to-interpret view of the success or failure of file transfers. Additionally, this simplification can make it easier to create charts or metrics related to the status of transfers, such as count of successful transfers, success rate, etc.

<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/dahsboard-sprint4.png" /></h1>     
     
### :heavy_check_mark: RNF 11: Tests
     
#### 1. Test file organization:
- Test files are located in the "tests" directory of the project.
- The test file names follow the naming pattern "*test.py" or "test*.py," which is compatible with the pytest test discovery pattern.

#### 2. Usage of pytest:
- The test structure is based on the pytest testing framework.
- The "pytest.ini" file is used to configure pytest behavior.
- The configuration file specifies the test file naming patterns, test directories, and other configuration options, such as filtering deprecation warnings.
- Markers are used to categorize tests. In the provided example, two markers are defined: "unit" and "requests."

#### 3. Usage of test libraries and modules:
- The `pytest` library is imported for writing tests.
- The `unittest.mock` library is imported for creating mocks and patches in tests.
- The `pytest` library is also used for handling exceptions and making assertions in tests.
- The `os.path` library is imported for checking file existence in the file system.
- Other project-specific modules and classes are imported to test their functionalities.

#### 4. Usage of fixtures and mocks:
- The `mocker.patch.object` function is used to replace objects and methods during tests, allowing for the simulation of specific behaviors.
- The `unittest.mock` library is used to create mock objects and define expected behaviors for method calls.
- The `mocker` object is passed as an argument to test methods to provide mocking and patching capabilities.

#### 5. Test class structure:
- Each test class is a subclass of `pytest` or `unittest.TestCase`, depending on the testing framework used.
- Test methods are prefixed with `test_`.
- The `@pytest.mark` annotation is used to mark tests with specific markers.

#### 6. Unit tests:
- The `TestAzureConnection` class contains tests for the `AzureConnection` class.
- The tests validate different connection scenarios with the Azure service and the expected responses.       
     
<span id="burndown">
    
## :chart_with_upwards_trend: Burndown

The monitoring of activities, which is the responsibility of the Scrum Master, is shown in the image below, which contains the Burndown chart generated by the team (where the X axis is the days worked in the sprint and the Y axis values represent the deliveries and efforts made with the over time), including the number of activities carried out.
    
- Ideal Line (Red)
- Royal Line (Blue)
    
<div align="center">
    
![Burndown Chart](https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/burndown-04.06.png)
</div>

- Graph updated on 6/04/2023
  
<br>
  
<span id="backlogs">

## :dart: Backlogs, Epics & User Stories

<h1 align="center"> <img src = "https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/documenta%C3%A7%C3%B5es-po.png" /></h1>

<br>
  
→ [Back to the top](#topo)
