# Summary

## Overview
This project has chosen the company, Web Puppies, which is one of the leading web development and digital solutions companies in Southeast Asia. It is a vendor company which provides various services for its clients that cater specifically to their needs. The project drills down on their key service, which is the provision of web development solutions and identifies how this business process can benefit from proper data management.

## Process
The process begins with a client/company approaching Web Puppies requesting a website to be developed showcasing all relevant information about their company and its operations. The result of the process is a fully developed and operational website for the client/company in accordance with the agreement between the business development representative and the client/company. As the terms of the contract between both parties ends upon the client receiving a fully functional and operational website, the result is discrete and clearly identifiable.

### AS-IS Diagram

While the process can run smoothly as depicted in the AS-IS swimlane diagram, the problems/gaps arise when there are complications to the process. 

1.	The fundamental issue with the current process is that all interactions with the client take place through one actor i.e. the business development representative. The company takes a traditional project management approach where stakeholders are only involved at specific milestones through the process. Although it minimizes the client’s interaction with various representatives from the Web Puppies team, it is time-consuming and inefficient to route all changes through one employee. Given the nature of the project and descriptive changes involved, feedback from either Web Puppies or the client could be lost-in-translation when it is communicated to the other party. In a realistic scenario, the client will likely go through several drafts of both the web design and mockup before agreeing to the final version of the website increasing the chances of miscommunication.

2.	The process lacks an internal database system which could streamline the process if integrated. The existing process will face roadblocks if the business development representative is unable to perform. For example, there could be potential delays in the process if the business development representative is unable to attend a meeting with the client to secure feedback or a meeting to convey client’s feedback to the Web Puppies team. Furthermore, the lack of a database system hinders the company from having a bird’s eye view on the case progress or tracking specific information about the case.  




## Result
The project resulted in the building of a database system using SQL to integrate Web Puppies' records  using MariaDB, executed SQL queries to extract status of product orders from the database and identified process inefficiencies for optimization.


### TO-BE Diagram
To fix the gaps identified, the business process has been amended as outlined below. The changes introduced in the TO-BE diagram are highlighted in green in the swimlane diagram.

#### 1. Assignment of Client team to handle incoming job orders
In the TO-BE diagram, the business development representative accepts and loads the request into the company’s database. Thereafter, the case is assigned to a client team comprising a website designer and a web developer. This team is directly involved in meeting the client’s brief and preparing mock-up websites as well as seeking and assessing possible implementation of client feedback. The TO-BE process also includes a specific pre-agreed number of meetings between the client and the website team to limit the possible iterations of revisions to the draft web designs and website mockups.

#### 2. Introduction of database system
The lack of a consolidated space comprising detailed insights into each client order is rectified with the introduction of a database system. This system allows all information related to a specific client order to be consolidated and updated at the time of the event/action taking place. In the TO-BE diagram, all updates to the case by each stakeholder have been keyed in real-time onto the database system. This also includes feedback from the clients on the draft web design and website mock-up, thereby allowing all parties to view the feedback simultaneously.

#### 3. Creation of tables and records on SQL
A total of 7 tables were created on SQL and thereafter, records were loaded into these tables. They are Client with 21 records, JobOrder with 22 records, Product with 21 records, Portfolio with 23 records, Employee with 31 records, FinanceDepartment with 22 records and Invoice with 22 records.
