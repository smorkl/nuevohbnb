# New HBnB V2

This project is a simulation of a rental platform similar to HBnB. In this application, users can:
- Create and manage accounts.
- Create and list amenities.
- Create places.
- Leave reviews for the places they visit.

Data is stored in a database using **SQLAlchemy**, which supports CRUD operations to save and manage users, amenities, places, and reviews.

## Table of Contents
1. [Installation](#installation)
2. [Usage](#usage)
3. [Project Architecture](#project-architecture)
4. [File Structure](#file-structure)
5. [Requirements](#requirements)
6. [Authors](#authors)

## Installation

1. Clone the repository:
    ```bash
    git clone git@github.com:smorkl/holbertonschool-hbnb.git
    cd part2
    cd HBnB
    ```

2. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Configure your database environment variables (if applicable) in the `config.py` file.

## Entities
- **User**: Represents a platform user.
- **Responsibilities**: Create and manage users, handle authentication information.
- **Example Methods**:
- `User.get_user_by_email(email)`: Retrieves a user by their email address.

- **Place**: Represents a property or accommodation available on the platform.
- **Responsibilities**: Define key information about the property, such as location, price, and amenities.
- **Example Methods**:
- `Place.add(place_data)`: Adds a new place to the database.
- `Place.get(place_id)`: Retrieves a place by its ID.

- **Review**: Represents a review made by a user about a place.
- **Responsibilities**: Allow users to leave comments and rate places.
- **Example Methods**:
- `Review.add(review_data)`: Adds a new review to a specific place.

- **Amenity**: Represents a service or feature that a place can offer.
- **Responsibilities**: Describe the services available at a place.
- **Example Methods**:
- `Amenity.add(amenity_data)`: Adds a new amenity to the database.

## Usage

To run the project, open a terminal and execute the following command:
```bash
git clone https://github.com/smorkl/project-HBNB.git
```
```bash
cd backend
python3 run.py
```
```bash
cd frontend
python -m http.server 8000
```
## Project Architecture

The project follows a three-layer architecture pattern, which helps keep the code organized, scalable, and modular:

- **Presentation Layer (API)**: Manages HTTP requests and responses.
- **Business Logic Layer (Services)**: Handles business logic and coordinates operations between models.
- **Persistence Layer (Repository)**: Interacts with the database to perform storage and retrieval operations.

## File Structure

```plaintext
hbnb/
├── app/
│   ├── __init__.py                 # Main module initialization
│   ├── api/
│   │   ├── __init__.py             # API initialization
│   │   ├── v1/                     # API versioning (version 1)
│   │       ├── __init__.py         # API v1 initialization
│   │       ├── users.py            # Endpoints for handling users
│   │       ├── places.py           # Endpoints for handling places
│   │       ├── reviews.py          # Endpoints for handling reviews
│   │       ├── amenities.py        # Endpoints for handling amenities
│   ├── models/                     # Data model definitions
│   │   ├── __init__.py             # Models initialization
│   │   ├── user.py                 # User model
│   │   ├── place.py                # Place model
│   │   ├── review.py               # Review model
│   │   ├── amenity.py              # Amenity model
│   ├── services/                   # Services managing business logic
│   │   ├── __init__.py             # Services initialization
│   │   ├── facade.py               # Facade class for simplified logic handling
│   ├── persistence/                # Data persistence management
│       ├── __init__.py             # Persistence initialization
│       ├── repository.py           # Repositories for database interaction
├── run.py                          # Main file to run the app
├── config.py                       # Application configurations
├── requirements.txt                # Project dependencies
├── README.md                       # Project documentation
```

## Requirements

- Python 3.x
- SQLAlchemy
- Flask
- SQLlite

All specific requirements are listed in `requirements.txt`. Install them by running `pip install -r requirements.txt`.

## Author

- [Author sebastian meneses salazar]

---
