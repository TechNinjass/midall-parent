## 04/03/2023 to 04/23/2023

<span id="top">

<h1 align="center">:bookmark: Second Delivery - SPRINT 2</h1>

<p align="center">
     <a href="#goals">Sprint goals</a> &nbsp |&nbsp &nbsp
     <a href="#deliveries">Deliveries</a> &nbsp |&nbsp &nbsp
     <a href="#burndown">Burndown</a> &nbsp |&nbsp &nbsp
     <a href="#backlogs">Backlogs</a>
</p>

We have a challenge of authenticating the user through the cloud security token, we also developed a dashboard (v1) for analyzing the transferred data.
    
<span id="goals">
    
## :dart: Sprint Goals
The requirements (both customer and educational institution) covered for the second sprint are:
- **RF 05:** Creation of the screen for configuring the API access account (Drive and Azure)
- **RF 08:** Create dashboard to monitor executions (BI tool)
- **RF 14:** Delete the file when transferred
- **RNF 11:** Tests (Fatec Requirement)
- **RNF 13:** Improvements in the file listing (Date and Size)
    
<br>
 
**:link: Click the link below to view the *Kanban* of team activities:**
> [Kanban Projects GitHub](https://github.com/orgs/TechNinjass/projects/2)
  
<br>
    
<span id="deliveries">
  
## :heavy_check_mark: Deliveries
 
### :heavy_check_mark: RF 05: Creation of the screen for configuring the API access account (Drive and Azure)

We made the token access authentication screen between the clouds, this screen was important in this project for several reasons:

**Security:** Token authentication is a way to ensure that only authorized users can access the application and configure the necessary parameters for the download service. This helps protect the application from unauthorized access and ensures that only users with the proper permissions can use the functionality.

**Privacy:** When dealing with video files stored on a video platform, it is possible that these files contain sensitive or confidential information. Token authentication helps ensure that only authorized users can access and download these files, keeping this information private.

**Traceability:** The use of authentication tokens allows tracking and auditing user actions in the application. This can be useful for monitoring purposes, analyzing results and identifying possible errors or suspicious activity.

**Secure integration with external services:** Integration with video platform and cloud service for file transfer requires secure authentication to ensure data integrity and confidentiality. The use of authentication tokens helps establish this communication securely, protecting data during transfer.
    
<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/tela%20do%20token%20de%20acesso.png" /></h1>
    
### :heavy_check_mark: RF 08: Create dashboard to monitor executions (BI tool)
    
📊 We chose LuckerStudio to build the dashboard due to their expertise in app development as a service, streamlined user interface, error and alert management, data management and analytics skills, dashboard building experience, and technical and post-service support. reliable deployment.
    
1- Within LookerStudio, choose the Microsoft SQL Server connection method.
    
<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/1dash.jpg" /></h1>
    
2- [At this link](https://support.google.com/looker-studio/answer/11283389#zippy=%2Cneste-artigo%2Cmosrar-a-lista-de-endere%C3%A7os-ip) we managed to access the IP used by looker studio, and this must be released within the cloud (Azure).
    
<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/2dash.jpg" /></h1>
    
3- In the network settings, we release two IP ranges, as shown below.
    
<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/3dash.jpg" /></h1>
    
4- With these steps completed, we can fill in the data for the connection methods:
    
<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/4dash.jpg" /></h1>
    
## 📉 Dashboard Result v.1.0
    
- List of Transferred Files
- Period, Size and File Name filters.
- Measurement Indicators (Total, Average, Heaviest/lightest file)
- Format Indicators (Quantity, Average and Total Size)
    
<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/dashboardcompleto.jpg" /></h1>

### :heavy_check_mark: RNF 13: Improvements in file listing (Date and Size)
    
As suggested by the client in the Sprint 1 presentation, we formatted the date and file size in the list screen.
    
- Date set to BR standard
- File Size set to "MB"
    
### :heavy_check_mark: RF 14: Delete file on transfer
    
We developed a logic that causes the file to be deleted from Google Drive when transferred to Azure. Reasons why it might be important to consider deleting the original files after moving to another cloud in the project:
    
**Storage Space Saving:** Transferring files to another cloud may consume storage space on the source platform. By deleting the original files after transferring, you can free up storage space and optimize the use of available resources.

**Data Security:** Deleting the original files after transferring can help ensure data security. By removing the original files, you lessen your exposure to potential security risks such as unauthorized access or data leakage, especially if the files contain sensitive information.

**Data consistency:** By deleting the original files after the transfer, you avoid the possibility of having multiple versions of the same file, which can cause inconsistencies in the data and make it difficult to analyze and correctly interpret the results.
    
<br>
    
<span id="burndown">
    
## :chart_with_upwards_trend: Burndown

The monitoring of activities, which is the responsibility of the Scrum Master, is shown in the image below, which contains the Burndown chart generated by the team (where the X axis is the days worked in the sprint and the Y axis values represent the deliveries and efforts made with the over time), including the number of activities carried out.
    
- Ideal Line (Red)
- Royal Line (Blue)
    
<div align="center">
    
![Burndown Chart](https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/burndown-sprint2-2304.png)
</div>

- Graph updated on 04/23/2023
  
<br>
  
<span id="backlogs">

## :dart: Backlogs, Epics & User Stories

<h1 align="center"> <img src="https://github.com/TechNinjass/midall-parent/blob/main/docs/Images/Backlogs-3.png" /></h1>

<br>
  
→ [Back to top](#topo)
