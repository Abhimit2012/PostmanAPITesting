# PostmanAPITesting
Project Overview
This project focuses on testing an API that manages student data using Postman. The API allows for the retrieval and management of student information, including details such as student IDs, names, locations, phone numbers, and courses enrolled. The JSON data provided serves as the test dataset for API requests and responses.

Objectives
Validate API Endpoints: Ensure that all API endpoints are functioning correctly and return the expected data.
CRUD Operations Testing: Test Create, Read, Update, and Delete operations on the student data.
Data Integrity: Verify that the data returned by the API matches the expected data structure and values.
Error Handling: Check the API’s response to invalid requests and data.
Test Data
The following JSON structure represents the initial dataset for the project:

json
Copy code
{
  "students": [
    {
      "id": "1",
      "name": "john",
      "location": "india",
      "phone": "4561234569",
      "courses": [
        "java",
        "selenium"
      ]
    },
    {
      "id": "2",
      "name": "smita",
      "location": "kenya",
      "phone": "4561212334",
      "courses": [
        "java",
        "HTML"
      ]
    },
    {
      "id": "3",
      "name": "Sanna",
      "location": "USA",
      "phone": "0532254532",
      "courses": [
        "C language",
        "computer course"
      ]
    },
    {
      "id": "4",
      "name": "MARK",
      "location": "USA",
      "phone": "05442266495",
      "courses": [
        "java",
        "Python"
      ]
    },
    {
      "id": "5",
      "name": "SANJAY",
      "location": "India",
      "phone": "45258789522",
      "courses": [
        "java",
        "html"
      ]
    }
  ]
}
Test Cases
Retrieve All Students:

Endpoint: GET /students
Expected Response: List of all student objects in the dataset.
Retrieve a Single Student by ID:

Endpoint: GET /students/{id}
Expected Response: Student object with the specified ID.
Create a New Student:

Endpoint: POST /students
Request Body: JSON object representing the new student.
Expected Response: Confirmation message and the newly created student object.
Update an Existing Student:

Endpoint: PUT /students/{id}
Request Body: JSON object with updated student data.
Expected Response: Confirmation message and the updated student object.
Delete a Student:

Endpoint: DELETE /students/{id}
Expected Response: Confirmation message indicating successful deletion.
Error Handling for Invalid Requests:

Invalid ID: Test with a non-existing student ID.
Invalid Data: Test with malformed JSON or missing required fields.
Tools and Technologies
Postman: For creating and running API tests.
JSON: For data representation and manipulation.
API Documentation: To be provided or generated using tools like Postman or Swagger.
Expected Outcomes
All API endpoints should function as expected and return the correct data.
CRUD operations should be thoroughly tested to ensure data integrity.
Error handling mechanisms should be validated to ensure robust API behavior in the face of invalid requests.
Conclusion
This project will provide a comprehensive testing framework for the student management API, ensuring its reliability and correctness. By using Postman, we will automate and validate the API functionality, making it easier to identify and fix issues promptly.
