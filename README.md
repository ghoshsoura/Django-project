# Necessary Syntax for this Project
This project is structured with the help of some basic commands required to build and run a Django Application.
# To create a Django App:
## django-admin startproject [ProjectName]
# To navigate to project Directory:
## cd [ProjectFolder]

Congrats! Now your basic Django application is ready. One of the advantage of using Django is when we create an app, it automatically include necessary pre-writte code modules, configuration file, dependencies etc.So we don't have to worry about building it from the scratch! Also we need to do is to modify the file according to the projects requirements and then build it to test it. Also we can test out how the basic template page looks like as Django administration have their own logics implemented when we create an app. To execute a Django application we can use the following command.

# To run a Django Application:
python manage.py runserver [ProjectName]

This will start a localhost server on port 8000. There you can see a Django developer page containing various links for resources. By default the port on which Django runs is 8000, but we can change it according to our needs(in case if you have one application already running on 8000 then that can be a problem). All we need to do is to include the port number on which we want to test our application.

[In ProjectDirectory] - python manage.py runserver [ProjectName] [PortNumber]

# How to handle changes made to the existing code logics and configuration file.
It is obvious that for our project we don't want to use pre-defined code logics and configuration file as we need to implement the project logic using our own idea. So the changes will be made and each time a changes is made it is better to keep track of those changes in django database server so that in future if we want to recover a specific part, we can restore that from the checkpoint. So django supports a specific command for this.
# i) Makemigrations: - 
This will check for any changes made to the project files or configuartions file and accordingly will construct a file containing all changes record. To do this operation the following command syntax should be followed - 

[In ProjectDirectory] - python manage.py makemigrations

# ii) migrate: -
After we stored all the changes in form a python file by running the makemigrations command, it is time to migrate that changes record to the django database server. Django server keeps track of this changes and accordingly render the application page by integrating that changes into the pages. Otherwise, we will not be able to see the updated application. So this command is vital to finalise the migrations in a application. To do this operation, the following command syntax should be followed.

[In ProjectDirectory] - python manage.py migrate


# Django-project
This project is based on creating simple pet medicine respository system where details of every pet whether vaccinated or not are tracked. The system allows the user to verify his/her details at admin panel and after verification he/she will be able to store pet information in order to be listed in the site.

I assumed this project to integrated with the business needs for a online store managemanet and thus I named it as Wisdompets Medicine Store.
Wisdom Pet Medicine strives to blend the best in traditional and alternative medicine in the diagnosis and treatment of health conditions in companion animals, including dogs, cats, birds, reptiles, rodents, and fish. We apply the latest healthcare technology, along with the wisdom garnered in the centuries old tradition of veterinary medicine, to find the safest and most effective treatments and cures, while maintaining a caring relationship with our patients and their guardians.
