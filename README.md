# Project Title
**Data Loading and Data Pre-processing**

# Description
We will be calculating the distribution of 'Channel Type' by creating the function. Further, we will call and view the distribution.
Also, we will load the top 1000 records into separate CSV file and to the database in the table.

# Getting Started 
The below instructions will help with the project set up and running on your local machine for development and testing purposes.

# Pre-requisites
 You will need to install the below software for the Project

 1) Jupyter Notebook for Python ( Latest Version )
 2) MySQL ( Latest Version )
 3) MYSQL server ( Latest Version )

# Guidelines for installing the above software
  Step-by-step installation

  **Jupyter Notebook**
  
 **Step1**: Install Python. Make sure you have Python installed on your system. You can download the latest version of Python from the official Python website.
 **Step2:** Step 2: Open a Terminal or Command Prompt Open a terminal on Linux or macOS, or a command prompt on Windows.
 **Step3:** Step 3: Install Jupyter Notebook Run the following command to install Jupyter Notebook using `pip`
 **Step4:** After the installation is complete, you can verify that Jupyter Notebook is installed correctly by typing the    Jupyter Notebook
           command in your terminal or command prompt

  **MYSQL** 

  **STEP1:** Download MySQL Installer:
  Visit the MySQL Community Downloads page.
  Download the MySQL Installer for Windows.

  **STEP2:** Run the Installer:
  Run the downloaded installer.
  Choose the "Developer Default" setup type, which includes MySQL Server, MySQL Workbench, and other helpful tools.
  Follow the on-screen instructions to complete the installation.

  **STEP3:** Configure MySQL Server:
  During the installation, you'll be prompted to set up the MySQL Server. Choose a root password and remember it.

  **STEP4:** Complete the Installation:
  The installer will complete the installation process.

  **STEP5:** Verify Installation:
  Open MySQL Workbench to verify that the MySQL server is running.

**MYSQL Server**

**STEP1:** Download SQL Server Installer:
Visit the Microsoft SQL Server Downloads page.
Click on "Download now" for the edition you want (e.g., SQL Server 2019 Express).

**STEP2:** Run the Installer:
Once the installer is downloaded, run it.
The SQL Server Installation Center will open.

**STEP3:** Accept License Terms:
Read and accept the license terms.

**STEP4:** Complete the Setup:
Once the installation is finished, the SQL Server Management Studio (SSMS) will open.

**STEP5**: Connect to the Database:
Open SQL Server Management Studio.
Connect to the server using the authentication method and credentials you provided during installation.

# Running tests

We will create a function of channel type i.e. channeltype (). It will the data as an 'argument' 
def channeltype(data);

Then we will call and view the distribution of channelType 
dis=channeltype(df)

Now we will view the distribution
dis

# Breaking tests

Now we want to load the top 1000 records into separate CSV file to the database
We will use, 
top_1000 = df.iloc[0:1000] 

**NOTE:** iloc in Python stands for "integer location" and is a method for selecting data by integer indexing

SAVE the dataframe to a CSV file
top_100.to_csv ("top_1000_channels.csv" , index = false )

# Deployment

Connection with MySQL Server
We created a connection URL that specifies the database type, username, password, host, and the name of the database. We used the create_engine function to create a database engine, which will establish a connection to the specified MySQL database. The engine will allow you to interact with the database.

 # Disclaimer

We might get an issue while attempting the CSV file 
Example ERROR: invalid start byte
The solution to the above error: we will use (encoding='latin-1')





