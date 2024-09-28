# United Helpers Disaster Response Database

## Overview
The **United Helpers Disaster Response Database** is designed to assist the nonprofit organization, United Helpers, in efficiently managing volunteers and tasks related to disaster relief efforts. This database tracks essential information about volunteers, tasks, packing lists, packages, and items, ensuring a streamlined approach to disaster management.

## Entity-Relationship Diagram (ERD)
![ERD Diagram](![image](https://github.com/user-attachments/assets/45a523b9-1f59-44d0-9317-9a8225a68d69)
)

## Features
- **Volunteer Management**: 
  - Track personal details of volunteers (name, address, phone number).
  - Assign multiple volunteers to various tasks.
  - Log start and end times for volunteer assignments.

- **Task Management**: 
  - Each task is identified by a unique task code and characterized by a description, type, and status.
  - Support for various task types, including recurring tasks and packing tasks.
  - Tasks can exist without volunteers, and volunteers can be entered without assigned tasks.

- **Packing List and Package Management**:
  - Associate packing tasks with specific packing lists.
  - Each packing list details the contents of packages (e.g., medical supplies, child-care packages).
  - Track packages with unique IDs, creation dates, and total weights.
  - Log actual items placed in packages, ensuring every package contains at least one item.

- **Item Management**:
  - Each item is assigned an ID, description, value, and available quantity.
  - Track quantities of each item included in packages.

## Entity-Relationship Diagram (ERD)
The ERD visually represents the relationships between entities in the United Helpers Disaster Response Database. It includes the following entities:

1. **Volunteer**
   - Attributes: Volunteer ID, Name, Address, Phone Number

2. **Task**
   - Attributes: Task Code, Description, Task Type, Status, Start Time, End Time
   - Relationships: Assigned to Volunteers

3. **Packing List**
   - Attributes: Packing List ID, Name, Description
   - Relationships: Linked to Packing Tasks

4. **Package**
   - Attributes: Package ID, Creation Date, Total Weight
   - Relationships: Associated with a Task

5. **Item**
   - Attributes: Item ID, Description, Value, Available Quantity
   - Relationships: Included in Packages

## How to Use
1. **Database Setup**:
   - Install MySQL on your system.
   - Create a new database for the United Helpers Disaster Response Database.

2. **Create Tables**:
   - Use SQL scripts to create tables based on the ERD provided. Make sure to define primary keys, foreign keys, and relationships.

3. **Data Entry**:
   - Populate the database with volunteer details, tasks, packing lists, items, and packages.

4. **Data Retrieval**:
   - Use SQL queries to retrieve and manage data according to your needs.

5. **Reporting**:
   - Generate reports to track volunteer assignments, task statuses, and package distributions.

## Conclusion
This database will help United Helpers effectively manage their resources and streamline their disaster response efforts. For any questions or contributions, feel free to reach out.
