![N|Solid](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/65f4a1dd9c51265f49d0.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240213%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240213T042955Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b641a1b0c070cb999cf45480565132680db852328c318536e12497f85b20e2fd)

# 0x00. AirBnB clone - The console

# Description
This the first step to create a command interpreter to manage your AirBnB objects and it calls the console, it allows the users to manage the entities of the system using the commands explained in this manual.
The users like the administrator of the Airbnb clone has the posibility of the creating and updating and managing objects and data of the application, those objects are:
 
 * Users
 * Places
 * States
 * Cities
 * Amenities
 * Reviews

This abstraction will also allow you to change the type of storage easily without updating all of your codebase.
The console will be a tool to validate this storage engine.

![N|Solid](https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2018/6/815046647d23428a14ca.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240213%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240213T042955Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8f8ad46708d33d98e6c552daa026b280ad45bda9f92308606bd23bd05f081b2f)

# How to use the console:

To use the console:
* you can start by running the console.py file:
    ```bash
    ~/AirBnB_clone$ ./console.py
    (hbnb) 
    ```

* `(hbnb) help`: this is the help command or it can be used next to one of the command for further help:
    ```bash
    (hbnb) help
    
    Documented commands (type help <topic>):
    ========================================
    EOF  all  create  destroy  help  quit  show  update
    
    (hbnb)
    ```
* `(hbnb) create <Model's name>`: this command can be used to create a model, it returns model's id:
    ```bash
    (hbnb) create BaseModel
    b6a6e15c-c67d-4312-9a75-9d084935e579
    (hbnb)
    ```
* `(hbnb) all <Model's name>`: this command can be used to display all the existent models:
    ```bash
    (hbnb) all BaseModel
    ["[BaseModel] (b6a6e15c-c67d-4312-9a75-9d084935e579) {'id': 'b6a6e15c-c67d-4312-9a75-9d084935e579', 'created_at': datetime.datetime(2023, 12, 9, 22, 21, 32, 216883), 'updated_at': datetime.datetime(2023, 12, 9, 22, 21, 32, 216883)}"]
    (hbnb)
    ```
* `(hbnb) show <Model's name> <model's id> `: this command follow by the id of the model, display only the content of that specific model:
    ```bash
    (hbnb) show BaseModel b6a6e15c-c67d-4312-9a75-9d084935e579
    [BaseModel] (b6a6e15c-c67d-4312-9a75-9d084935e579) {'id': 'b6a6e15c-c67d-4312-9a75-9d084935e579', 'created_at': datetime.datetime(2023, 12, 9, 22, 21, 32, 216883), 'updated_at': datetime.datetime(2023, 12, 9, 22, 21, 32, 216883)}
    (hbnb)
    ```
* `(hbnb) destroy <model's name> <instance's id>`: this command can delete a model using it's instance id.
    ```bash
    (hbnb) destroy User b6a6e15c-c67d-4312-9a75-9d084935e579
    (hbnb) 
    ```
* `(hbnb) update BaseModel <model's id> <attribute>: <the new value>`: this command can be used to update the value of an attribute using it's id.

* `(hbnb) quit`: this command can be used to exit the console.
    ```bash
    (hbnb) quit

    ~/AirBnB_clone$ 
    ```
## AUTHORS
 

* **Arabah Imrane** - [arabahimrane](https://github.com/arabahimrane)
* **PortFolio** - [Web sit](https://imranearabah.com/)