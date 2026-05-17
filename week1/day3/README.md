# Day 3 - Data Modeling

## 1. Basic Concepts
- **App** - Group of tabs. Ex: Sales App
- **Object** - Table to store data. Ex: Student
- **Record** - One row of data. Ex: John Doe
- **Field** - Column in table. Ex: Email

## 2. Standard vs Custom
- **Standard Object** - Built by Salesforce. Ex: Account, Contact
- **Custom Object** - We create. Ex: Student__c, Course__c

## 3. College Data Model
**Objects:** Student, Faculty, Course, Department

**Relationships:**
- Student → Department = Lookup
- Faculty → Department = Lookup  
- Course → Department = Lookup
- Student ↔ Course = Many-to-Many

## 4. Formula Fields
1. **Full Name** = First Name + Last Name - Auto combine names
2. **Remaining Seats** = Total Seats - Enrolled - Auto calculate vacancy
3. **Age** = Today Year - Birth Year - Auto update age

## 5. Validation Rules
1. **Email Required** - Email cannot be blank
2. **Valid Age** - Age between 5 to 100 only
3. **Seat Limit** - Enrolled students cannot exceed total seats

## 6. Why Not Excel?
Excel has no relationships, no validation, duplicate data, manual work, no security. 
Salesforce gives structured data with objects, relationships, formulas and validation. So data is clean and automated.
