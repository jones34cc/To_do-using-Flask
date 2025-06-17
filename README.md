# To-Do List API

A simple Flask-based API for managing a to-do list.

## Installation

1. Clone the repository:
```
git clone https://github.com/your-username/to-do-list-api.git
```
2. Navigate to the project directory:
```
cd to-do-list-api
```
3. Create a virtual environment and activate it:
```
python3 -m venv venv
source venv/bin/activate
```
4. Install the required dependencies:
```
pip install -r requirements.txt
```

## Usage

1. Start the Flask development server:
```
python api.py
```
2. The API will be available at `http://localhost:5000/`.

## API

### Get All Items
- **Endpoint:** `/items`
- **Method:** `GET`
- **Response:** Returns a list of all to-do items.

### Get a Specific Item
- **Endpoint:** `/items/<int:item_id>`
- **Method:** `GET`
- **Response:** Returns the to-do item with the specified `item_id`.

### Create a New Item
- **Endpoint:** `/items`
- **Method:** `POST`
- **Request Body:** `{"name": "New Item", "description": "This is a new item."}`
- **Response:** Returns the newly created to-do item.

### Update an Existing Item
- **Endpoint:** `/items/<int:item_id>`
- **Method:** `PUT`
- **Request Body:** `{"name": "Updated Item", "description": "This item has been updated."}`
- **Response:** Returns the updated to-do item.

### Delete an Item
- **Endpoint:** `/items/<int:item_id>`
- **Method:** `DELETE`
- **Response:** Returns a success message.

## Contributing

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature`.
3. Make your changes and commit them: `git commit -am 'Add some feature'`.
4. Push to the branch: `git push origin feature/your-feature`.
5. Submit a pull request.


## Testing

To run the tests, execute the following command:
```
python -m unittest discover tests
```
