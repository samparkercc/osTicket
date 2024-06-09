<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Learn how to set up:
    - Roles
    - Departments
    - Teams
    - Agents
    - Users
    - SLA
    - Help Topics
 
    <h2>Post-Install Configuration Pre-Reqs</h2>
- [osTicket: Prerequisites and Installation](https://github.com/samparkercc/osTicket-prereqs1/tree/main)


<h2>Configuration Steps</h2>

<p>
1.) Configure Roles
    - Login using the username and password you filled in on the setup page. 
<p>
<img width="486" alt="Screenshot 2024-06-09 at 3 46 58 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/02363d6c-7341-47b3-8bd0-62269956d7e4">
<p>
    - Go to Admin Panel -> Agents -> Roles
<p>
<img width="963" alt="Screenshot 2024-06-09 at 3 47 24 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/33b1dd68-5b68-4bcb-a06a-6cd9d59bd1e5">
<p>
    <img width="964" alt="Screenshot 2024-06-09 at 4 16 20 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/6f6ed3aa-9600-4ea5-9a49-664846cf76c1">
    <p>
    - Add New Role -> Fill in name "Supreme Admin" -> Permissions -> Check all boxes in "Tickets" -> Create Role
    <p>
    <img width="960" alt="Screenshot 2024-06-09 at 4 18 38 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/4f988ed4-c6cb-4245-bff5-441a6c14e632">

<p>
<img width="961" alt="Screenshot 2024-06-09 at 4 20 48 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/ca148ca5-f20b-4daa-8d05-9f8a5a693f94">
<p>
2.) Configure Departments 
    - Admin Panel -> Agents -> Departments
    <p>
    <img width="952" alt="Screenshot 2024-06-09 at 4 27 58 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/789a2283-c378-4e81-a857-38af3416b67a">
<p>
    - Add New Department -> Select Parent: -Top-Level Department- -> Fill in name "System Administrators" -> Create Department 
    <p>
    <img width="954" alt="Screenshot 2024-06-09 at 4 31 24 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/37d922dd-affe-4041-a0fc-b4da19262a45">
<p>
3.) Configure Teams
    - Admin Panel -> Agents -> Teams
    <p>
    <img width="958" alt="Screenshot 2024-06-09 at 4 39 29 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/bfb41623-0147-4e8b-9daf-fc3cada81779">
    <p>
    Add new Team -> Fill in name "Level II Support" -> Create Team 
    <p>
    <img width="954" alt="Screenshot 2024-06-09 at 4 43 28 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/dc8b15a8-ebe7-448b-ac75-45d51eeac264">
<p>
NOTE: If Level I Support is not already created, then go ahead and create that team as well. 
<p>
4.) Allow anyone to create tickets
    - Admin Panel -> Settings -> User Settings 
<img width="960" alt="Screenshot 2024-06-09 at 4 48 10 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/0a82be81-15f6-4ba5-aaaf-8107c8ef8dd8">
<p>
    - Make sure there is no registration required and the method is public. 
    <p>
    <img width="954" alt="Screenshot 2024-06-09 at 4 59 58 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/e57ea4e5-6ecf-474d-b06f-cc9c1f75d596">
<p>
5.) Configure Agents (workers)
    - Admin Panel -> Agents 
<p>
<img width="955" alt="Screenshot 2024-06-09 at 5 02 21 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/cd01472f-434f-4c4b-bd21-6504d859f749">
<p>
    - Add New Role -> Fill in: Name -> Email -> Username -> Set Password (Uncheck two boxes since we are using this for test purposes) 
    <p>
    <img width="960" alt="Screenshot 2024-06-09 at 5 06 04 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/b64d1657-d65f-40b8-ad9d-24d73c35c9eb">
<p>
<img width="646" alt="Screenshot 2024-06-09 at 5 09 16 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/65bc5809-f60a-44cb-b841-abd180d029ce">
<p>
    - Access -> Select Department "System Administrators" -> Select Role "Supreme Admin" 
    <p>
    <img width="961" alt="Screenshot 2024-06-09 at 5 11 26 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/f91886bd-63d4-4f5c-bc0f-11564195bf1d">
<p>
    - Teams -> Select Team "Level II Support" -> Add -> Create 
    <p>
    <img width="957" alt="Screenshot 2024-06-09 at 5 11 37 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/cede3bf8-1563-497c-9559-ad14f1289a63">
<p>
    - Repeat steps for Account page except exchange Jane Doe for John Doe. 
    <p>
    <img width="961" alt="Screenshot 2024-06-09 at 5 21 16 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/45cb9d43-bc88-469e-b595-7eec479ad963">
<p>
    - Access -> Select Department "Support" -> Select Role "View Only" -> Create 
    <p>
    <img width="957" alt="Screenshot 2024-06-09 at 5 22 25 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/8677f0b0-a4ae-472f-b138-9c72a9cfdf45">
<p>
6.) Configure Users (customers) 
    - Agent Panel -> User Directory 
      <p>
      <img width="960" alt="Screenshot 2024-06-09 at 5 27 05 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/5c791e60-40f7-4765-84f7-9637aef64493">
  <p> 
    - Add New User -> Fill in Email -> Fill in Name -> Add User 
      <p>
      <img width="645" alt="Screenshot 2024-06-09 at 5 32 51 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/52860c1d-91f3-4637-bdef-3eabaad3abe8">
  <p>
    - Repeat previous steps with a new name 
      <p>
      <img width="644" alt="Screenshot 2024-06-09 at 5 35 17 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/a190987a-9518-4249-b88e-4287d2713f3d">
  <p>
  7.) Configure SLA 
      - Admin Panel -> Manage -> SLA
      <p>
      <img width="958" alt="Screenshot 2024-06-09 at 5 37 47 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/9eb2568b-01e1-484d-890a-94a531a701e4">
<p>
    - Add New SLA Plan -> Name, "Sev-A" -> Grace Period, "1" (hour) -> Schedule, "24/7" -> Add Plan 
    <p>
    <img width="958" alt="Screenshot 2024-06-09 at 5 38 49 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/d8587658-6c1f-482d-864d-a26786f3268b">
<p>
<img width="961" alt="Screenshot 2024-06-09 at 5 40 32 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/e0a8aa82-675d-45eb-bfeb-e08ce77b2ff0">
<p>
    - Add New SLA Plan -> Name, "Sev-B" -> Grace Period, "4" (hour) -> Schedule, "24/7" -> Add Plan
<p>
<img width="955" alt="Screenshot 2024-06-09 at 5 53 38 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/e8ec95ca-eee6-4c0b-8caa-0bb13d442334">
<p>
    - Add New SLA Plan -> Name, "Sev-C" -> Grace Period, "8" (hour) -> Schedule, "Monday - Friday 8am - 5pm with U.S. Holidays" -> Add Plan
    <p>
    <img width="957" alt="Screenshot 2024-06-09 at 5 58 17 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/f34bb54f-bdf4-4829-ab18-c3ab8ef32f39">
    <p>
8.) Configure Help Topics
    - Admin Panel -> Manage -> Help Topics
        <p>
        <img width="959" alt="Screenshot 2024-06-09 at 6 01 28 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/c2e5b0d0-3b89-46e0-887c-1b389633a6d5">
<p>
    - Add New Help Topic -> Topic, "Business Critical Outage" -> Add Topic 
    <p>
        <img width="957" alt="Screenshot 2024-06-09 at 6 03 26 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/6ef39d8f-d389-4aca-8c42-10bb84125cd5">
<p>
    <img width="956" alt="Screenshot 2024-06-09 at 6 04 58 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/80b7e9dd-9699-4540-a5bc-accf50af4dff">
<p>
    - Add New Help Topic -> Topic, "Personal Computer Issues" -> Add Topic 
<p>
<img width="960" alt="Screenshot 2024-06-09 at 6 09 07 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/8362be25-cb99-4aa5-bacf-60b1b54019e6">
<p>
    - Add New Help Topic -> Topic, "Equipment Request" -> Add Topic 
    <p>
    <img width="961" alt="Screenshot 2024-06-09 at 6 10 28 PM" src="https://github.com/samparkercc/osTicket-Post-Installation-Configuration/assets/171518500/b18fc915-79ed-4eba-8348-799c83aecdbc">
<p>
    - Add New Help Topic -> Topic, "Password Reset" -> Add Topic
<p>
We've now setup: 
    <p>
    - Roles
        <p>
    - Departments
    - Teams
            <p>
    - Agents
<p>
    - Users
    <p>
    - SLA
    <p>
    - Help Topics
<p>
Congratulations! We have now setup a ticketing system! From here, you can test out how a ticketing system works by submitting tickets with different topics, SLA's, assigning to different departments/teams, etc. 
<p>
Great job!
