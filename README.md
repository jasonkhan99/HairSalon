# _Hair Salon_

#### _C# Database basics code review for Epicodus, 07/31/2020_

#### By _**Jason Khan**_

## Name

_You've been referred by Pierre to his friend Claire who is the owner of a hair salon called Eau Claire's Salon. She has contracted you out to create an MVC web application to help her manage her employees (stylists) and their clients. Claire should be able to add a list of stylists working at the salon, and for each stylist, add clients who see that stylist. The stylists have specific specialties, so each client can only see (belong to) a single stylist._

## Setup/Installation Requirements

  1. Click on this [link to the project repository](https://github.com/jasonkhan99/HairSalon.git) on GitHub.  
  2. Click on the "Clone or download" button to copy the project.     
  3. If you know how to use the command line and Github, clone the project with `git clone`. Use "**Download ZIP**" if not.
  4. Extract the Zip to a folder of your choice and open with a code editor (i.e. vscode)
  5. Import the .sql file into a SQL Manager as a Database. In mySQL Workbench you import from self-contained file and select the .sql file
  6. Make sure your database matches this Schema:  

  DROP DATABASE IF EXISTS \`FirstName_LastName\`;  
  CREATE DATABASE \`FirstName_LastName\`;  
  USE \`FirstName_LastName\`;  

  CREATE TABLE \`Clients\` (  
    \`ClientId\` int(11) NOT NULL AUTO_INCREMENT,  
    \`Name\` varchar(255) DEFAULT NULL,  
    \`StylistId\` int(11) NOT NULL,  
    PRIMARY KEY (\`ClientId\`)  
  DELETE CASCADE  
  ) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4  
  COLLATE=utf8mb4_0900_ai_ci;

  CREATE TABLE \`Stylists\` (  
    \`StylistId\` int(11) NOT NULL AUTO_INCREMENT,  
    \`Name\` varchar(255) DEFAULT NULL,  
  PRIMARY KEY (\`StylistId\`)  
)  ENGINE=InnoDB DEFAULT CHARSET=utf8mb4   COLLATE=utf8mb4_0900_ai_ci;

  7. Navigate to the HairSalon directory by entering `cd` **Your Filepath/**`HairSalon`. Then enter `dotnet restore`, `dotnet build`, and `dotnet run` into the terminal.

## Known Bugs

_No known bugs_

## Support and contact details

_https://github.com/jasonkhan99_

## Technologies Used

* C#
* .NET-Core 2.2
* ASP.NET Core MVC
* Entity Framework Core
* MySql
* Visual Studio Code
* GitHub

### License

*This site is licensed under the MIT license.*

Copyright (c) 2020 **_{Jason Khan}_**