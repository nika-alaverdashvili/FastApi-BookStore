# FastApi-BookStore

FastAPI Bookstore API is a web-based application designed to manage and organize the collection
of a virtual bookstore. It allows users to perform CRUD (create, read, update, delete) operations
on books. Most importantly, only authorized users can add, modify, and delete books, while unauthorized
users can only read. The API also supports user authentication for secure access to protected endpoints.

## Features

- User can register and authenticate.

- **User Authentication**: Secure user registration and login using JSON Web Tokens (JWT). Users can obtain access tokens to protect themselves when accessing secure API endpoints.

- Both authorized and unauthorized users can read books, they can also filter books by condition, author, genre and owner filter.
  
- Authorized users can add books to the bookstore database. Each book entry contains essential information such as title, author, genre, description, condition, location, image, and owner.

- Authorized users can update the information of existing books through ID, and the record update must include the necessary information such as the method of posting.

- Authorized users can delete books by: specifying the books ID.

- Responses are returned in JSON format.


## Usage


### Follow these steps to set up and run the FastAPI project on your local machine:


## Running Tests

To run tests, run the following command

Clone the Repository:
```
git clone https://github.com/nika-alaverdashvili/FastApi-BookStore
```
Navigate to the Project Directory:
```
cd .\FastApi-BookStore\
```

Create a Virtual Environment:
```
python -m venv venv
```

Activate the Virtual Environment on windows:
```
venv\Scripts\activate
```

Install Project Dependencies from requirements.txt:
```
pip install -r requirements.txt
```
Start the FastAPI Server:
```
uvicorn src.main.main:app --reload
```
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
- Access the API Documentation:

Open your web browser and navigate to http://localhost:8000/docs. You will be presented with interactive Swagger documentation that allows you to explore and interact with the API endpoints.
Explore the API:

- Use the Swagger documentation to test the different API endpoints, such as creating, updating, and deleting books, as well as user registration and login.
