2025 QA to BE Conversion Program - Final Project
Objective
Constraint
Business Requirement
Use Case API
Technical Requirement
Sequence Diagram
Register Login Auth Logout
Process
Project Competition
Objective
To get hands-on experience in building end to end Java and Spring project from scratch
Learning opportunity to incorporate all the material learned during bootcamp
Simulate real world software engineering process
Constraint
Individual project
Will not be scored or evaluated
Can use cursor or antigravity (or other AI vibe code tools), but you need to understand how
the generated code works
Business Requirement
Build online marketplace platform
Use Case API
customer can register, login
customer password should be hashed using built-in password hash library from spring
framework
password validation should also use this built-in validation library from spring framework
login can use oauth token in JWT/JWS, use symmetric/asymmetric key
customer can search product, view product list and view product detail
search product and view product list result should be paginated
search can support wildcard search
customer can add product to shopping cart
must be logged-in
no need for inventory stock checking, assume stock is unlimited
customer can view shopping cart and delete product from shopping cart
must be logged-in
login session validation via jwt cookie or jwt header
customer can logout
invalidate jwt token and/or cookie after logout
Technical Requirement
minimum 4 microservices: api gateway, member, product and cart
only need to develop API, no need to build UI or client side
use API gateway for authN and authZ implemented also as java web
search can be performed in postgres or mongodb directly (use elasticsearch is optional, only
if you want more challenge)
use java and spring
use postgres for relational, mongo for document and redis for cache, (you can decide
between relational or document based, which one is more suitable for each microservice
domain model structure)
write unit test and integration test
data size:
member: minimum 5,000 members
product: minimum 50,000 products
Sequence Diagram
This is only an example to help planning, does not have to be exactly made this way
Register Login Auth Logout
Process
fork this repo to your gdncomm gh account, and PR back to this repo
GitHub - gdncomm-andi-r-djunaedi/training-project-202511
follow blibli git flow with release branch and feature branch on your fork repo
and PR back the release branch to the original repo
can add your squad lead and team member as code reviewer to help review your code
design and development timeline: 5 days 15 december 2025
Project Competition
Best 3 project from each development site (best 3 from Jakarta and best 3 from Bangalore with
total 6 project) will be selected to present their project, you can consider this as Mini Hackathon
Judge
Phani
Andi
Shandy
Project Evaluation Criteria
Functional completeness and correctness, zero or minimum bugs
System design API Design, DB Design)
Code cleanliness, structure and organization
Non Functional aspect consideration such as security, performance, observability, testability,
etc
Extra Challenge Optional, for those who likes to live on the bleeding edge)
All microservices dockerized, can run on Kubernetes
Use ElasticSearch or SolR for Search data store
Use gRPC instead of REST API
Implement Design Pattern in your code, should be well suited with the problem solved but not
reinvent the wheel
