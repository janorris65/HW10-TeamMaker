# Givens
GIVEN a command-line application that accepts user input
WHEN I am prompted for my team members and their information
THEN an HTML file is generated that displays a nicely formatted team roster based on user input
WHEN I click on an email address in the HTML
THEN my default email program opens and populates the TO field of the email with the address
WHEN I click on the GitHub username
THEN that GitHub profile opens in a new tab
WHEN I start the application
//THEN I am prompted to enter the team manager’s name, employee ID, email address, and office number
WHEN I enter the team manager’s name, employee ID, email address, and office number//
//THEN I am presented with a menu with the option to add an engineer or an intern or to finish building my team//
//WHEN I select the engineer option
THEN I am prompted to enter the engineer’s name, ID, email, and GitHub username, and I am taken back to the menu//
//WHEN I select the intern option
THEN I am prompted to enter the intern’s name, ID, email, and school, and I am taken back to the menu//
WHEN I decide to finish building my team
THEN I exit the application, and the HTML is generated
# Specifics 
Important: Make sure that you remove dist from the .gitignore file so that Git will track this folder and include it when you push up to your application's repository.
# Classes
The application must include Employee, Manager, Engineer, and Intern classes. The tests for these classes (in the _tests_ directory) must ALL pass.
## Employee 
The first class is an Employee parent class with the following properties and methods:


name


id


email


getName()


getId()


getEmail()


getRole()—returns 'Employee'

## Others
The other three classes will extend Employee.
In addition to Employee's properties and methods, Manager will also have the following:


officeNumber


getRole()—overridden to return 'Manager'


In addition to Employee's properties and methods, Engineer will also have the following:


github—GitHub username


getGithub()


getRole()—overridden to return 'Engineer'


In addition to Employee's properties and methods, Intern will also have the following:


school


getSchool()


getRole()—overridden to return 'Intern'


Finally, although it’s not a requirement, consider adding validation to ensure that user input is in the proper format.