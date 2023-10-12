"# api" 
John Rey D. Pascua

# JSON POST with Database Integration

This JSON POST API endpoint allows clients to send structured data to the server for creating or updating records, providing flexibility and ease of use. The server responds with HTTP status codes and relevant JSON data upon processing, serving various purposes such as user registration, data updates, and custom workflows with secure authentication. For detailed requirements and error-handling procedures, refer to the official documentation.

## API Description

This API simplifies tasks, providing smooth data handling, instant communication, and secure third-party integration. It offers strong authentication, a scalable structure, and detailed documentation, enabling developers to build flexible and effective apps for improved functionality and user engagement.

Purpose:
Our API is designed to simplify intricate tasks and elevate your application's performance, be it a website, mobile app, or other software. It provides a powerful toolkit to streamline processes, enhance user satisfaction, and increase efficiency.

Key Features:

Effortlessly manage data with support for various types and secure storage.

Ensure protected data transmission and storage.

Implement strong user authentication and fine-tuned access control.

Protect API endpoints based on roles and permissions.

Enable real-time communication, including messaging and live updates with efficient protocols.

Seamlessly integrate with third-party services like social media and payment gateways.

Generate in-depth analytics and reports to understand user behavior and system performance.

Scale with a reliable architecture, redundancy, and continuous support.

Comprehensive documentation, security measures, and customization options.

Prioritize error handling and offer a robust foundation for diverse applications.

## API Enpoints

Explain the accessible endpoints, their roles, and the necessary inputs.

http://127.0.0.1/api/public/

Purpose: This endpoint is for inserting new data into the database and requires the parameters "First name" and "Last name" to do so.

http://127.0.0.1/api/public/postUpdate

Purpose: This endpoint is for updating current database entries and requires "ID," "First name," and "Last name" as input parameters.

http://127.0.0.1/api/public/postPrint

Purpose: This endpoint is for retrieving and displaying data stored in the database, and it doesn't require any input parameters.

http://127.0.0.1/api/public/postDelete

Purpose: This endpoint is designed for deleting particular data from the database and necessitates the "ID" parameter for this purpose.



## Request Payload



## JSON Payload postName:

- Request payload:
{
  "lname":"hortizuela",
   "fname":"manny"
}

This payload is used for creating a new name entry. It requires both the last name ("lname") and first name ("fname") of the person being added.

## JSON Payload printName:
 
- Request payload:

This payload does not contain any specific fields. It might be used for retrieving or printing a name from the system, but the payload itself does not specify any required or optional fields.

## JSON Payload updateName:

- Request payload:
{
  "id":1,
  "lname":"wick",
   "fname":"john"
}

This payload is used for updating an existing name entry identified by the specified "id". It requires the updated last name ("lname") and first name ("fname") of the person.

## JSON Payload deleteName:

- Request payload:
{
  "id":1
}

This payload is used for deleting a name entry based on the specified "id". It only requires the unique identifier of the name entry to be deleted.


 


## Response


## JSON Payload postName:

- Response payload:
{
         "status":"success","data":null
}

"status": Indicates the status of the API request. In this case, it's "success" indicating that the request was successful.
"data": This field is present but set to null, indicating that no specific data is returned for successful postName requests.

## JSON Payload printName:

- Response payload:
{
         "status":"success","data":["lname":"hortizuela","fname":"manny","lname":"licayan","fname":"arnold"]
}

"status": Indicates the status of the API request. It's "success" indicating that the request was successful.
"data": An array containing objects, each representing a name entry. Each object contains "lname" (last name) and "fname" (first name) fields with corresponding values. The response includes multiple name entries.


## JSON Payload updateName:

- Response payload:
{
         "status":"success","data":null
}

"status": Indicates the status of the API request. It's "success" indicating that the request was successful.
"data": This field is present but set to null, indicating that no specific data is returned for successful updateName requests.


## JSON Payload deleteName:

- Response payload:
{
         "status":"success","data":null
}

"status": Indicates the status of the API request. It's "success" indicating that the request was successful.
"data": This field is present but set to null, indicating that no specific data is returned for successful deleteName requests.


 


## Usage


Open Postman:
Make sure Postman is installed and running on your computer.

Insert Data with a POST Request:
To add data to the database using the /api/public/postName endpoint:

Select the POST HTTP method.
Input the URL: http://127.0.0.1/api/public/postName.
In the request body, provide the values for the "fname" and "lname" parameters.
Click "Send" to send the request.
Update Data with a POST Request:
To modify existing database entries using the /api/public/postUpdate endpoint:

Choose the POST HTTP method.
Enter the URL: http://127.0.0.1/api/public/postUpdate.
Include the updated values for the "id," "fname," and "lname" parameters in the request body.
Click "Send" to submit the request.
Display Data with a POST Request:
To view database data using the /api/public/postPrint endpoint:

Use the POST HTTP method.
Specify the URL: http://127.0.0.1/api/public/postPrint.
Leave the request body empty as no additional parameters are necessary.
Click "Send" to send the request.
Delete Data with a POST Request:
To delete data from the database via the /api/public/postDelete endpoint:

Set the HTTP method to POST.
Input the URL: http://127.0.0.1/api/public/postDelete.
In the request body, provide the "id" parameter with the ID of the data you want to delete.
Click "Send" to initiate the request.

## License
No License 



## Contributors

Sir Manny Hortizuela
provided:

- some codes
- database structure
- payloads
- etc.

## Contact
Include contact
information for inquiries or support.

John Rey D. Pascua
- johnreypascua1111@gmail.com
- johnrey.pascua@student.dmmmsu.edu.ph
- 09568595337
