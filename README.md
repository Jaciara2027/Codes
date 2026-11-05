# Codes
This Repository Contains the majority of the codes that i did durring my summer trainnig.


# Project Structure – API Stock
The API Stock is organized into clear layers to keep responsibilities separated and the codebase maintainable. Each layer has a single job: the Controller handles HTTP requests and format validation, the Service contains business rules, the Repository communicates with the database through stored procedures, and the database itself enforces data integrity.

The solution can be arranged as a single project with folders (simpler to start) or as multiple projects in one solution (more scalable). In the single‑project layout, the main folders are:

Controllers – receive HTTP requests, validate input format (such as regex for email or barcode), and return appropriate responses.

Services – implement business logic, including required fields, length limits, stock rules, and other domain‑specific validations.

Repositories – call the stored procedures using Dapper or SqlCommand and map the results back to the application.
