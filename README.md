# DataScience
This is a repository of some projects developed related with vulnerabilities data science as environment study part of the System&amp;Computer Engineering profesisonal program. It contains a series of projects developed using Python and Jupyter Notebooks for handling various tasks related to computer security and data analysis. Below is a description of each of the projects:


---

# Developed Projects
## 1. API Consumption

### Description:
This project focuses on consuming different APIs to obtain relevant information for computer security analysis.

### Used Libraries:
- **Requests**: For making HTTP requests to the APIs.
- **JSON**: For handling responses in JSON format.

### Key Functions:
- `requests.get()`: To make GET requests to the APIs.
- `json.loads()`: To load response data into a Python dictionary.


## 2. JSON Structuring Management
### Description:
It addresses the handling and analysis of structured data in JSON format, with the aim of extracting useful information for further analysis.

### Used Libraries:
- **JSON**: For handling data in JSON format.

### Key Functions:
- `json.loads()`: To load a JSON string into a Python dictionary.
- `json.dumps()`: To convert a Python dictionary into a JSON string.


## 3. Use of Microsoft Azure Platform
### Description:
This project explores the use of the Microsoft Azure platform for creating NoSQL database instances and data processing from Jupyter Notebooks.

### Used Libraries:
- **Azure SDK for Python**: For interacting with Azure services from Python.

### Importations
- from azure.cosmos import CosmosClient, exceptions:

  **Cosmos Client**: This is the main database interactive class for Python, allowing realize the basic read, create, update and delete operations for a document in a Cosmos DB database
  **exceptions**: A module that contains specified expresions to be launched throught an Azure Cosmos DB interactions, as for example 'CosmosHttpResponseError', to verify when there's an error from a HTTP request to Azure Cosmos DB
  
- from azure.cosmos.partition_key import PartitionKey:
  The PartitionKey import develops the data scalability and distribuition eficienty. As more exactly being a class, it's used for stablish the partition key to the order of a document content
  

## 4. Detection of "Bluekeep" Vulnerabilities

### Description:
This project focuses on consuming vulnerability APIs and CVE reports to detect the vulnerability known as "Bluekeep", using IP addresses as input and storing the results in NoSQL databases in Microsoft Azure.

### Used Libraries:
- **Requests**: For making HTTP requests to vulnerability APIs.
- **Azure SDK for Python**: For interacting with Azure services.

### Key Functions:
- `requests.get()`: To obtain information about vulnerabilities from the API.
- `azure.cosmos.cosmos_client.CosmosClient.create_database()`: To create a NoSQL database in Azure.

## 5. Software Vulnerability Detection

### Description:
It involves consuming vulnerability APIs and CVE reports to detect vulnerabilities in different software, storing the results in NoSQL databases in Microsoft Azure.

### Used Libraries:
- **Requests**: For making HTTP requests to vulnerability APIs.
- **Azure SDK for Python**: For interacting with Azure services.
- **MITRE & VulnDB Apis**: For performing port scans on provided IP addresses.

### Key Functions:
- `requests.get()`: To obtain information about vulnerabilities from the API.


## 6. Tracing Installed Software on Computers

### Description:
This project focuses on tracing software installed on computers by consuming vulnerability APIs and CVE reports, storing the results in NoSQL databases in Microsoft Azure.

### Used Libraries:
- **from windows_tools.installed_software import get_installed_software**: Complies part of a library called windows_tools, which provides specific functionalities for interacting with Windows operating systems from Python.
  
### Key Procedure:
- for software in get_installed_software():
    print(software['name']):
Prints the name of each software installed on the Windows system, using the get_installed_software() function in the windows_tools library to get that information.

## 7. Data Visualization Management

### Description:
It involves the visualization of data obtained from CVE reports, providing useful visualizations for vulnerability analysis, and storing the results in NoSQL databases in Microsoft Azure.

### Used Libraries:
- **Matplotlib**: For creating charts and data visualizations.
- **Pandas**: For handling structured data.

### Key Functions:
- `matplotlib.pyplot.plot()`: To plot a line chart.
- `pandas.DataFrame.plot()`: To create charts from data stored in a DataFrame.

---

This README file provides an overview of the projects developed in this repository, including technical details about the libraries used and key functions in each project. Each project includes its own detailed documentation and the necessary code files for execution.

Thank you for reviewing our projects! If you have any questions or suggestions, feel free to contact us.
