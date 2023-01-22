# Flask Store REST API with Flask, SQLAlchemy, Flask-Smorest, Flask-JWT-Extended, and Database migration with Alembic and Flask-Migrate

This project is a Flask Store REST API that uses Flask for API development, SQLAlchemy for database management, Flask-JWT-Extended for authentication. The API also includes Swagger UI for documentation and testing. 

This API all it will do is it will receive the store data, add it to the database and then return the information that it added. When we create items, we're gonna receive a POST request to /store/ the store name in this case, it's my store /item. So this is the endpoint. And it will receive the name and price of the item that we want to create. And it will create this item inside the store. Then it will respond with the item that it created. This response may not seem particularly useful since it's just the data that the client sent us, but it's important to confirm to the client that the request was successful. And this is a way to do that. By responding with the information that the API now has, the client can make sure that it contains everything that it expects. To retrieve all the stores and all their items. We will send a GET request to /store. Note that to create a store. This was a POST request to /store. Now this is a GET request to /store. And this responds with an object or a dictionary containing the stores key, that is a list. And inside this list, there is a bunch of dictionaries. Each dictionary represents one store that has the name and the items. So in this case, we would have a list of items with a single dictionary, which is the item we already created. If you wanted to get a particular store, you can do /store/ and then the name of the store, that's a GET request. And that just sends the information for a single store, which is the same as what was included here in this list but just for the one store that was requested. And if you wanted to get the items within a store, you can do /store/ the store name and then item. And that will get you the list of items within the store.

## Installation

To install the necessary dependencies for this project, run the following command:

```bash
pip install -r requirements.txt
```

This will install all the necessary libraries and modules.

## Running the Project

To run the project, Run the following command:

```bash
flask run
```

This will start the Flask development server and allow you to access the API from your local machine.