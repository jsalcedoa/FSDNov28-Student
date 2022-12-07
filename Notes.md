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
