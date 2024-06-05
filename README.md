# simple-webapp
Learning to create a simple backend for web application using Java without any Spring features.

## Learning goals
For what need Spring is created.
Basics of servlets, endpoints, services, domain objects and Tomcat.
Basics of backend.

## Sources
Based largely on learnings from Marco Behler's course "The confident Spring professional" https://www.marcobehler.com/ which I bought for myself in order to understand the fundamentals of Spring. After going through the course twice going at it for the third time. Minimal comments for clarity, checking source code only when necessary.

## Use
Endpoints for local use:
- GET "/" returns html greeting
- GET "/invoices" returns all posted invoices as JSON
- POST "/invoices?user_id=jeff&amount=40" creates an invoice and returns it as JSON
- POST "/*" returns 404 
