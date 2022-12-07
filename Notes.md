# Class Notes

## Class Project

- We won't actually build it but will work through the process

## Docker

- <https://docs.docker.com/engine/reference/builder/>
- <https://hub.docker.com/_/microsoft-windows-base-os-images>
- https://docs.docker.com/storage/volumes/
- https://antman-does-software.com/techs-surprisingly-bad-math-in-team-design

### Stateful data

- data that persists and is available across containers

## Project Candidates

1. Doctor office reservation shceduling app 1 11 1 1 1
2. App to allow people to buy food that delivery services can't deliver 1
3. Google maps for parking spaces 1 1 1 1 1  1
4. Password manager  11
5. Task management system
    

## CICD

- https://en.wikipedia.org/wiki/Robotic_process_automation

## Design Lab 1

1. Account balance
2. transactions
3. Account types
4. users
5. how the customer is accessing the account
6. Notifications
7. Statements
8. Reciepts 
9. specific transactions


### Domain Model

1. Account
    - accounts have a balance
    - types of accounts

2. Transactions
    - credit/debit/query
    - deposit/withdraw/transfer/query
    - account
    - users
3. Generated data
    - reciept
    - statements
    - notifications
4. Sources
    - teller
    - mobile
    - web
    - atm
5. Account Holder
6. Bank card

## issues

1. Bank Account
    - associated with user
    - balance
    - type (tbd)
    - Status
    - account number
    - associated to bank card

2. Need a connection to the actual data source

3. Currency type

- {
    currency: USD,
    amount: 289882
}

## Structural rules

1. Well formed - all the right pieces are there in the right cardinality

2. Valid - according to the business rules all value  legal or allowed

## Architecture

- Have to consider source

## Robustness

1. Lifecycle - legal data constrainst
2. External  account transaction 

### Test cases 
####  a - b
- a == b
- a >b
- b >  a

---

## Dec 2 - Java

- James Gosling on Youtube

### Patterns
- hillside.net
- https://github.com/iluwatar/java-design-patterns

#### Factory
- Abstract product and abstract maker

---

## Spring Boot Playground

- https://github.com/atharvasiddhabhatti/Springboot-Playground

## Maven 
- https://maven.apache.org/guides/getting-started/index.html

## Jenkins 
- https://www.jenkins.io/
- the batch file is in c:\tools\Jenkins
- https://www.jenkins.io/doc/book/pipeline/syntax/

- USA United States, Les etats unis, Untied States of America
- Chili CHile

---
## Data

- https://hibernate.org/orm/

---

## Doctor office apt app.

- Create appointments for patients at a doctors office
- provide upates to patients and doctors about the status
- change the scheduling or other data of appoint


- What are the domain objects?
    - Schedule - Health Care "slate" 
    - Health care worker - Nurse, Tech, DOctors (specialists, GP)
    - Patients  - They are under our care
    - Referral 
    - Appointment
        - Health care workers
        - Patient
        - Time and date

- Slating microservice
    - Managing the schedule of health care workers.
    - slate for a health for a specific perios
    - availability for a HCW for a period
    - Is anyone available at a partical time who is allowed to see that patient (speciality)

- Patient Management Mirco service
    - fetch patient medical records
    - update medical record
    - add a new patient
    - make patients inactive 

- Appointments
    - Transaction microservices
    - Create an appointment(patient(s), HCW(s), time/date, duration, location)
    - Cancel an appointment
    - Modify an appointment
    - Display appointment info

- Reception microservice
    - Message = appointment request.
    - Comes from the user interface.
    -

### User stories

1. Patient calls in to book an appointment, receptionst confirms they are a patient, asks for the reason, finds the right doctor and available time and date and confirms
2. Docter requests an appointment
3. Rec has to postpone and appointment or change doctor
4. Patient has canceled

### data design

- Message to sent over REST inteface
- List of messages
- Appoointment, appointment request, slating request, insurance request.
- How you write a validator to ensure these object

### Dev design
- Where are our git repos, what sort of branching would
- Writing a production piple
- How do we test this?
- What are the processes in our app - different thread? 
- Are any applicable design
- What parts should go into docker containers?



---

## Data Service

- Takes CRUD requests from an application 
- Translates this into a data format appropriate for the implementation
- Different models
    - RDBM sytems - structured data is full defined by a schema - tabular form
    - NoSQL - Semi-structed


