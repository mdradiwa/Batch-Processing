# PySpark Installation
Here I want to share how to install PySpark.
## Dependencies
Dependencies of PySpark for Windows system include:

- JAVA
- Python
- PySpark
- Winutils

## Installation
### 1. Download and Install Java
Install the latest version of the JAVA from https://www.java.com/en/download/. Then after installation, check it via command prompt and type `java --version`,

![image](https://user-images.githubusercontent.com/124119569/225222641-7ec46dab-5182-4aa3-9f54-4b7277021a4f.png)

### 2. Download and Install Python
Install Python from https://www.python.org/downloads/. Run the downloaded file for installation, make sure to check the “include python to Path” and install the recommended packages (including ‘pip’). To see python is already installed you can go to command prompt and type `python --version`,

![image](https://user-images.githubusercontent.com/124119569/225222355-a2fc5be9-7eeb-47d6-bf47-0b40b82a96d3.png)

### 3. Download and Unzip PySpark
Download PySpark via this link https://spark.apache.org/downloads.html and unzip it.

**Note:** The location of my file where I extracted are here,

![image](https://user-images.githubusercontent.com/124119569/225222971-3fd761be-f89a-4189-85d1-ee0ccd35440b.png)

### 4. Download winutils.exe
In order to run Apache Spark locally, winutils.exe is required in the Windows Operating system. This is because Spark needs elements of the Hadoop codebase called ‘winutils‘ when it runs on non-windows clusters. 

Here is the link where I download winutils https://github.com/kontext-tech/winutils.

Create a folder structure hadoop\bin within the (C:) disk and put the downloaded winutils.exe file there.

![image](https://user-images.githubusercontent.com/124119569/225224028-c98252f7-b3d1-46db-aeae-557aa480a089.png)

### 5. Set Environment Variables
In order to set the environment variables

- Go to Windows search
- Type “env” —it will show the “edit environment variable for your account”, click on it
- Click on “New” for the user variables and add the following variable name and values (depending upon the location of the downloaded files)

![image](https://user-images.githubusercontent.com/124119569/225224516-f1f0d806-18f2-4962-8378-53f6d7e15d59.png)

![image](https://user-images.githubusercontent.com/124119569/225224593-48722fe3-7d08-4c58-b729-b0e8b0681460.png)

![image](https://user-images.githubusercontent.com/124119569/225224659-e557832a-af77-4c81-bddb-cf86a3a199a4.png)

Next, Update the PATH variable with the \bin folder address, containing the executable files of PySpark and Hadoop. This will help in executing Pyspark from the command prompt.
- Click on the “Path” in system variable

![image](https://user-images.githubusercontent.com/124119569/225224949-2dc810b9-e9c0-4e74-a59b-c4feed63bcc5.png)

-Then add the following two values ( we are using the previously defined Environment variables here)
%SPARK_HOME%\bin
%HADOOP_HOME%\bin 

![image](https://user-images.githubusercontent.com/124119569/225225243-0e7ba5ec-fbcb-4d95-9a0e-eec9e123a59e.png)

### 6. Let's try Spark!
Test if PySpark has been installed correctly and all the environment variables are set.

Go to command prompt, then type `pyspark`,

![image](https://user-images.githubusercontent.com/124119569/225220884-b339ed62-6828-4ca8-9591-82d967b69ff3.png)

Great! The PySpark is installed. To see the PySpark running well, go to “https://localhost:4040” without closing command prompt,

**Note:** My localhost name are hp, so the link will be https://hp:4040

![image](https://user-images.githubusercontent.com/124119569/225227039-00f1acad-0363-42e0-8adb-ba8203ab8d55.png)

