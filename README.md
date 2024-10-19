# SOC Incident Management and Response Lab using NIST 800 61 Framework (Privilege Escalation)
<p align="center">

  ![Screenshot 2024-10-19 121305](https://github.com/user-attachments/assets/147c3199-2bf5-4eb4-8edd-dd7fa387c8f2)

</p>

In this lab, I managed and responded to security incidents within Azure Sentinel following the NIST 800-61 Incident Management Lifecycle. I started by analyzing detected alerts, setting severity levels, assigning owners, and investigating timelines and related events to determine whether incidents were legitimate (True Positive) or false alarms. For valid incidents, I applied containment, eradication, and recovery measures using automated playbooks. Finally, I documented my findings and closed the incidents in Sentinel. This lab demonstrates my ability to effectively manage and respond to security incidents in a structured SOC environment.




<h2>Environments and Technologies Used</h2>

- Microsoft Sentinel


<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1 - Preparation
- (We initiated this already by ingesting all of the logs into Log Analytics Workspace and Sentinel and configuring alert rules)

- Step 2 - Detection & Analysis 
- Step 3 - Containment, Eradication, and Recovery
- Step 4 - Document Findings/Info and Clouse out the Incident in Sentinel


<h2>Deployment and Configuration Steps</h2>

- Step 2: Detection & Analysis (You may have different alerts/incidents)
- Set Severity, Status, Owner
  ![Screenshot 2024-10-19 173229](https://github.com/user-attachments/assets/6a33268a-a6b0-4ee9-9028-c6b9661c8cb4)

- View Full Details (New Experience)
  ![Screenshot 2024-10-19 173408](https://github.com/user-attachments/assets/3df92c3d-4a6a-482b-92ee-8436e16183a8)

- Observe the Activity Log (for history of incident)
  ![Screenshot 2024-10-19 173610](https://github.com/user-attachments/assets/0dca36cc-ee64-412c-a2b7-85deb4e75404)

- Observe Entities and Incident Timelines (are they doing anything else?)
  ![Screenshot 2024-10-19 173706](https://github.com/user-attachments/assets/fe08a67e-c03e-4a46-81ed-39f2a26c1b73)
  ![Screenshot 2024-10-19 173716](https://github.com/user-attachments/assets/ad4f1b39-b283-4487-9544-4dccc06f7f96)


- “Investigate” the incident and continue trying to determine the scope
  ![Screenshot 2024-10-19 173931](https://github.com/user-attachments/assets/d980a0c4-9f65-45eb-ada3-482e24ec8af2)

- Inspect the entities and see if there are any related events
  ![Screenshot 2024-10-19 174035](https://github.com/user-attachments/assets/0550b7b8-7858-4114-b822-8e9fe9c5b17c)

- Determine legitimacy of the incident (True Positive, False Positive, etc.)
- If True Positive, continue, if False positive, close it out

  (In a real case scenario, to determine if this incident is legit or not, I would ping the employee on Microsoft Teams asking him a series of questions which would determine if an alert like this would be a false positive or not.)


