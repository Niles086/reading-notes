# Readings: CRUD

Status Codes Based On REST Methods

In one's own vernacular, articulate the representation of each category of status codes:

100’s: Informational responses. These signify that the request has been acknowledged and comprehended, yet further processing is imperative.
200's: Responses of triumph. These denote that the request was victorious, and the sought-after operation has been concluded.
300's: Responses of redirection. These communicate that the desired resource has been relocated to a new address, necessitating the client to reroute accordingly.
400's: Responses to client errors. These reveal that the client submitted a faulty request, impeding the server from fulfilling the operation.
500's: Responses to server errors. These reveal that the server encountered an impediment, impeding the execution of the request.
Exploration of Specific Status Codes:

Status Code 202: A code that signifies the acceptance of a request for processing, though the execution has yet to reach completion.
Status Code 308: Denotes that the requested resource has permanently migrated to a novel URL, prompting the client to update bookmarks and direct future inquiries to the updated location.
Handling Update without Data: To signify an update without returning data to the client, one would employ the 204 No Content status code.
Discerning Resource Existence:

Status Code 404: If a resource formerly existed but is now absent, the appropriate code is 404 Not Found.
Deciphering 'Forbidden':

Status Code 403: The Forbidden status code indicates that while the client has authorization to access the server, it is barred from accessing the specified resource.
Videos
Constructing a REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

Securing Database Credentials:
Why is it imperative to extricate the MongoDB database string from the server and sequester it in the .env file?

Enhanced Security: Safeguarding sensitive information, such as database credentials, outside the codebase averts inadvertent exposure and unauthorized access.
Simplified Configuration Management: Centralizing environment variables in a .env file streamlines configuration across diverse environments (development, testing, production).
Reduced Code Clutter: Maintaining code clarity and focus on functionality by segregating configuration details.
Understanding Middleware:

Middleware Defined: Middleware serves as an intermediary between the client and the core application logic, facilitating tasks such as logging, authentication, validation, and data transformation pre or post-request.
Modularity and Reusability: Middleware fosters code reusability by encapsulating common functionality in distinct modules, paving the way for enriched application features without direct alterations to application logic.
Express Middleware:

app.use(express.json()): This middleware parses JSON data from POST and PUT request bodies, making it accessible in the req.body object. Essential for handling JSON-based APIs, it enhances code readability by structuring request data.
Route Parameter Meaning:

/:id in a Route: Serves as a placeholder for a dynamic value, enabling routing for individual resources based on specific identifiers. This dynamic routing allows for flexibility in handling various resource IDs.
Distinguishing Between PUT and PATCH:

PUT vs. PATCH: PUT replaces the entire resource, while PATCH selectively updates specific portions. Optimal method selection ensures precision and efficiency in data manipulation.
Setting Default Values in a Schema:

Default Values: Defining default values for optional fields guarantees that a field possesses a value, averting potential errors due to missing data. This approach simplifies data handling and promotes code cleanliness.
Interpreting 500 Error Status Code:

500 Internal Server Error: Indicates that the server encountered an unforeseen error, necessitating debugging by reviewing server logs to identify and rectify the issue. Clients may retry the request based on the specific error and recovery strategy.
Differentiating Status Codes 200 and 201:

Status Code 200 (OK): Signifies a successful request with completed operations.
Status Code 201 (Created): Signifies a successful request resulting in the creation of a new resource, providing explicit information about the outcome.