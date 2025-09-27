# ER Diagram Workshop – Submission Template

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
<img width="912" height="1041" alt="Screenshot 2025-09-27 090859" src="https://github.com/user-attachments/assets/00ef1e25-bf5f-4cea-98e5-01ee4b63dff8" />



### Entities and Attributes

- Member (ID, Name, Contact, MembershipType, StartDate) - Trainer (ID, Name, Contact) - Program (Yoga, Weight Lifting, Zumba Dance) - Equipment - Payment (PaymentID) - Gym - Staff 
Attributes: - Member  ID, Name, Contact, MembershipType, StartDate - Trainer  ID, Name, Contact - Program  ProgramName (Yoga, Zumba, Weight Lifting) - Payment  PaymentID 
Relationships: - Member <-> Trainer (Trains) - Member <-> Equipment (Uses) - Trainer <-> Program (Tasks) - Program <-> Payment (Session) - Trainer <-> Gym (Has) - Gym <-> Staff (Has) 

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
<img width="721" height="735" alt="image" src="https://github.com/user-attachments/assets/4ff25a23-f7bc-4ae3-9f31-d7137aa716e8" />


### Entities and Attributes

The Central Library wants to manage both book lending and cultural events. 
Requirements: 

Members borrow books, with loan dates and return dates tracked.  
Each book has details such as title, author, and category.  
The library organizes events; members can register for them.  
Each event has one or more speakers/authors.  
Rooms in the library are booked for events and study purposes. 
Overdue fines apply for late book returns.

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

<img width="903" height="1042" alt="Screenshot 2025-09-27 091026" src="https://github.com/user-attachments/assets/0a53be2e-0572-44f3-ba2c-c09d477ef77f" />

### Entities and Attributes

This ER Diagram represents a restaurant meal ordering system. 
Entities: 
1. Chef: - Attributes: chef_id, chef_name, chef_salary - Relationship: prepares Meal 
2. Meal: - Attributes: Meal_name, Meal_price - Relationship: consists_of Ingredients - Prepared by Chef 
3. Customers: - Attributes: Cust_id, Cust_name, Cust_address, Cust_phone - Relationship: orders Meal 
4. Ingredients: - Attributes: ing_name, Description 
5. Supplier: - Attributes: S_id, S_name, S_city - Relationship: attends Ingredients 
Relationships:- Chef prepares Meal- Customers orders Meal- Meal consists_of Ingredients - Supplier attends Ingredients. 


## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
