AirBnB Clone v2

This project is a group effort aimed at developing an AirBnB clone using Python with an Object-Oriented Programming approach for the back-end. We utilize MySQL for data storage and management, employing SQLAlchemy ORM for seamless interaction.

### Technologies Used:
- Python for Back-end
- Flask as the Web Framework
- MySQL for Database
- SQLAlchemy ORM for data handling

### Usage:
1. Clone this repository to your local machine.

2. To run the program:
   - For MySQL storage:
     ```
     $ HBNB_MYSQL_USER=hbnb_dev HBNB_MYSQL_PWD=hbnb_dev_pwd HBNB_MYSQL_HOST=localhost HBNB_MYSQL_DB=hbnb_dev_db HBNB_TYPE_STORAGE=db ./console.py
     ```
   - For FileStorage:
     ```
     $ ./console.py
     ```

3. Upon running the command, you'll be greeted with a prompt `(hbnb)` indicating you're in the HBnB console.

### Commands:
- **create**: Create an object of a specified class.
- **show**: Display details of an object based on its ID.
- **destroy**: Delete an object based on its ID.
- **all**: Display all objects of one type or all types.
- **quit/EOF**: Exit the console.
- **help**: Get descriptions of available commands.

### Supported Classes:
- BaseModel
- User
- State
- City
- Amenity
- Place
- Review

### Additional Features:
- Utilize the following syntax for more streamlined commands:
  - `<class name>.<command>(<parameters>)`, e.g., `City.show(my_city_id)`
- Named parameters are supported:
  - `<command> <class name> (<named_parameters>)`, e.g., `create Amenity name="WiFi"`
