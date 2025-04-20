# java-springboot
This project is a simple web application which can perform CRUD operations on employee details using Springboot framework
Tools and versions:
Springboot - 3.4.4
maven - 3.9.9
java - 17
Database - h2

# Setup for running app locally
STEP 1: Install Chocolatey (Only once)[This can make installation easy]
        Open PowerShell as Administrator, then run:
        Command : Set-ExecutionPolicy Bypass -Scope Process -Force;
                  [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.SecurityProtocolType]::Tls12;
                  iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

STEP 2: Install Java JDK 17
        Command : choco install openjdk17 -y
        Verify Java: 
        Command : java -version

STEP 3: Install Maven
        Command : choco install maven -y
        Verify Maven:
        command : mvn -v
        
STEP 4: Setup Spring Boot App
        first install Git
        Command : choco install git -y
        Then : 
        Command : git clone https://github.com/YOUR_USERNAME/employee-management-springboot.git
                  cd employee-management-springboot

STEP 5: Run the Spring Boot Application
        From the project folder: 
        Command : mvn clean install 
                  ![image](https://github.com/user-attachments/assets/1b39a258-20e7-4dbf-a000-3d7cd9457f4a)
                  mvn spring-boot:run

# After running app test the app by
Opening this url in your browser: http://localhost:8080
- for database access open url : http://localhost:8080/h2-console
               set jdbc url to : jdbc:h2:mem:testdb

Happy Execution!!!
