# Employee-Managment
This project is developed by Balaram Paradhan.
==============================================
how to run this project
=======================
After the downloading the project, To run the project in the local system.
--> Do install angul cli and node application running the command npm install @angular/cli.
--> After that do inm instal for fullfill the dependencies.
--> install bootstrap by running the command install bootstrap
--> do install ngx pagination for getting the pagination.
--> Also check for the updated version node by running the command node -v
--> After installation of the all plugins run the command ng serve. 
what the Empployee management project contains
==============================================
   The Employee mangement based on Modular approach it contains four modules
   a)Auth module
   b)Dashboard Module
   c)Employee Module
   d)App module (default)
   
   
a)Auth module
==============
  The auth module contains Two component
    1)Login component
    =================
       --> The login component is contains the login form will very good look and feel with  form validtaion property,
       --> It has the input field for username and password field for fill the password with two buttons a)login b)Register.
    2)Register component
    ====================
       --> The Registration form contains the all field required for an registratioj form like
           Name,Id,Joindate,gender,city,country,state,gmail, with two buttons 1) regiter 2)cancel.
      --> The registation form also has the validation properties so that the user have fill all the fields.
      
b)Dashboard module
===================
  The Dashboard module contains only the dashboard component along with the routing file.
  ==> the dashboard module used to show the datails about employees like how many male are there and female are there and their documents also and the total employee nimber in an GUI format
  ==> In the dashboard compomenent we have used bootstrap card classes to make this look and feel and for better user experiance.
  ==> It will show the data dynamic based on the records stored in the database.
  ==>And also contains the service classes and routing Module.
  
c)Employee Module
================
   The employee module inside the pages folder contains Four components,And also contains the service classes and routing Module.
   
     1)Employee list
        |--AddEmployee
     2Edit-empployee
     3)view-Employee
     4)Delete Employee
     
  
  1)Employee list
  --------------- 
    --> The employee component is rsponsible for show all the employee according to the pagination of the page.
    --> This emloyee list is shown in the tablular format with the option for each employee which are edit,delete,view and with the plugin ngx pagination.
    --> by clicking the Edit button user can edit the employee by passing the id in the routing.
    --> by clicking the delte button user can delete the employee by passing the id in the routing form the database by makenbign the http calls or by using the service classes.
    --> by clicking the view button user can view the employee by passing the id in the routing.
    --> In the employee list component we have an button "addEmployee" by clicking this button we will naviaget to the add employee component,
        In the Add employee component we have all the label along with an additional fiels "image" where the employee cal upload the image.
  2)Edit-empolyee
  ----------------
    -->When you click the edit button in the Employee list compoenent you will navigate to this employee edit component page
    --> The Edit Employee component has all the required field for an employee and with two buttons 1)update 2)cancel
    --> by retrieving the "id" from route we are making the service calls to the details of the particular employee.
    --> In this component after fatching all the details for an paticular employee and fetching the details in the particular fields we can modify the employee properties and by presing the update button
        the component will do he service call for update the employee details 
    --> And by pressing the cancel button we will navigate to the employee list again.
  3)View employee
 ----------------
    --> The view employee component contains all the labels so to view show the details of the particular employee.
    --> After pressing the view button in the employee list component the route wil sent the id with in the route and after getting the paramenter from the route
        the view employee call the service class to get the data and display the data.
    --> In view Empliyee component we can only see the data we can not modyfy it.
    --> It contain only one button i.e "backToManu" which will navigate to the employee list.
    
  4)Delete Employee (button)
  -----------------
     --> The Delete employee  used to delete an secific or particular employee 
     --> when the user clickes the delete button show in the employee list component it calles the seervice class based on the id and do dlete the employee information permanently from the database
  
   d) App module
   ==============
   --> The App module is the first loading module.
   --> It contains one component "sidebar" which is used to navigate the route between module.
      
  
