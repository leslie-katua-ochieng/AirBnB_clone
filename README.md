# AirBnB_clone
Synopsis
The Airbnb clone project for which we are creating a copy of the Airbnb. Only some features will be implemented and will be listed below once completed.

Project Description
This is the first part of the AirBnB clone project where we worked on the backend of the project whiles interfacing it with a console application with the help of the cmd module in python.

Data (python objects) generated are stored in a json file and can be accessed with the help of the json module in python

Features
Command Interpreter
Description
The Command Interpreter is used to manage the whole application's functionality from the command line, such as:

Crete a new object.
Retrieve an object from a file, database, etc.
Execute operation on objects. e.g. Count, compute statistics, etc.
Update object's attributes.
Destroy an object.
Usage
To launch the console application in interactive mode simply run:

console.py 

or to use the non-interactive mode run:

echo "your-command-goes-here" | ./console.py 

Commands
Command	Description
quit or EOF	Exits the program
Usage	By itself
-----	-----
help	Provides a text describing how to use a command.
Usage	By itself --or-- help <command>
-----	-----
create	Creates a new instance of a valid Class, saves it (to the JSON file) and prints the id. Valid classes are: BaseModel, User, State, City, Amenity, Place, Review.
Usage	create <class name>
-----	-----
show	Prints the string representation of an instance based on the class name and id
Usage	show <class name> <id> --or-- <class name>.show(<id>)
-----	-----
destroy	Deletes an instance based on the class name and id (saves the change into a JSON file).
Usage	destroy <class name> <id> --or-- .destroy()
-----	-----
all	Prints all string representation of all instances based or not on the class name.
Usage	By itself or all <class name> --or-- <class name>.all()
-----	-----
update	Updates an instance based on the class name and id by adding or updating attribute (saves the changes into a JSON file).
Usage	update <class name> <id> <attribute name> "<attribute value>" ---or--- <class name>.update(<id>, <attribute name>, <attribute value>) --or-- <class name>.update(<id>, <dictionary representation>)
-----	-----
count	Retrieve the number of instances of a class.
Usage	<class name>.count()
Tests
If you wish to run at the test for this application all of the test are located under the test/ folder and can execute all of them by simply running:

python3 -m unittest discover tests 

from the root directory.

Bugs
No known bugs at this time.
Author
Leslie Ochieng 
Abel Appiah
