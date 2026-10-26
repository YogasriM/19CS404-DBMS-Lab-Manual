# ER Diagram Workshop – Submission Template
# YOGASRI M
# 212224220124

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management

**Business Context:**  
FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  
- Members register with name, membership type, and start date.  
- Each member can join multiple programs (Yoga, Zumba, Weight Training).  
- Trainers assigned to programs; a program may have multiple trainers.  
- Members may book personal training sessions with trainers.  
- Attendance recorded for each session.  
- Payments tracked for memberships and sessions.

### ER Diagram:
<img width="899" height="1599" alt="WhatsApp Image 2026-10-26 at 11 49 47 AM" src="https://github.com/user-attachments/assets/41e1fcce-a41f-4afc-8018-2c1d01659ccd" />

*Paste or attach your diagram here*

<img width="422" height="383" alt="image" src="https://github.com/user-attachments/assets/d6d9f9ab-1bd8-47c2-86f6-343f4cdf8464" />




![ER Diagram](er_diagram_fitness.png)

### Entities and Attributes

| Entity     | Attributes (PK, FK)                 | Notes                     |
| ---------- | ----------------------------------- | ------------------------- |
| Member     | ID (PK), Name, Age                  | Stores member details     |
| Session    | ID (PK), Date                       | Stores session details    |
| Trainer    | ID (PK), Name                       | Stores trainer details    |
| Program    | ID (PK), Name, Schedule             | Stores program details    |
| Payment    | Payment_ID (PK), Amount, Date, Type | Stores payment details    |
| Attendance | ID (PK), Status                     | Stores attendance details |


### Relationships and Constraints
| Relationship                  | Cardinality | Participation | Notes                                           |
| ----------------------------- | ----------- | ------------- | ----------------------------------------------- |
| Member — Session (Book)       | M:N         | Not specified | Members book sessions                           |
| Session — Trainer (Conducted) | 1:M         | Not specified | Sessions are conducted by trainers              |
| Member — Program (Join)       | 1:M         | Not specified | Members join programs                           |
| Program — Trainer (Assigned)  | 1:M         | Not specified | Programs are assigned to trainers               |
| Member — Payment (Make)       | 1:M         | Not specified | Members make payments                           |
| Trainer — Attendance (Take)   | 1:M         | Not specified | Trainers are associated with attendance records |

### Assumptions


# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:

<img width="1600" height="1382" alt="WhatsApp Image 2026-10-21 at 4 12 43 PM" src="https://github.com/user-attachments/assets/c828d852-de65-492d-acdc-befab9d5095a" />

*Paste or attach your diagram here*  

<img width="442" height="396" alt="image" src="https://github.com/user-attachments/assets/eb9ac7cb-86bb-4886-8e40-68980feda77f" />

![ER Diagram](er_diagram_library.png)

### Entities and Attributes

Entity	          Attributes (PK, FK)	                Notes
Books   	        Book_ID (PK), Name, Author	        Stores book details.
Loan	            Loan_ID (PK), Amount, Due	          Stores loan information.
Members           Mem_ID (PK), Name, Phone_No, Email	Stores member details.
Event	            Event_ID (PK), Name, Type, Date	    Stores event details.
Speakers/Authors	ID (PK), Name, Amount, Type	        Stores speaker or author information.
Room	            Room_ID(PK), Date, Type, Capacity	  Stores room details.



### Relationships and Constraints
| Relationship                   | Cardinality   | Participation | Notes                                 |
| ------------------------------ | ------------- | ------------- | ------------------------------------- |
| Books — Loan                   | Not specified | Not specified | Connects books and loans              |
| Loan — Members                 | Not specified | Not specified | Connects loans and members            |
| Event — Members (Register)     | M:N (assumed) | Not specified | Members register for events           |
| Event — Speakers/Authors (Has) | Not specified | Not specified | Connects events with speakers/authors |
| Event — Room (Booking)         | Not specified | Not specified | Connects events with rooms            |



### Assumptions
- 
- 
- 

---

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
*Paste or attach your diagram here*  

<img width="882" height="555" alt="image" src="https://github.com/user-attachments/assets/3acf160f-e603-4d8b-aad2-f19ad579e851" />


![ER Diagram](er_diagram_restaurant.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
