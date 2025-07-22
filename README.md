# Transistor
Application Setup
1. Download GTFS Data
Download the GTFS.zip file for the Netherlands. Import the contents into your MySQL database.

2. Configure the Database Connection
Open the DatabaseSingleton class and update the following lines with your database credentials:

Line 16: Database URL

Line 17: Username

Line 18: Password

3. Initial Data Cleanup (First Launch Only)
On your first launch, it's recommended to clean the database for optimal performance.
To do this, call the cleanData method inside mapGUI.main like so:

java
Copy
Edit
dataGetter.cleanData();
Important:
Running cleanData() may take a while. Once it has cleaned the database, remove this line to speed up future startups.

Running the Application
Launch the application by running the main method in the mapGUI class.

Enter two postcodes to calculate travel information.

Postcodes must be within the Maastricht area.

Invalid input will trigger an error message.

