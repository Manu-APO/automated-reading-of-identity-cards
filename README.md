# Employee Contracts Automation with Document Understanding :
## The automatization is composed of two processes:
1. **RobotReaderForIDs**:
* Extract data* from IDs images using Document Understanding (UiPath OCR)
* Validate the extracted data in UIPath Validation Station
* Create an output .xlsx file with the extracted data and add categorizes the IDs according to processing final status
2. **RobotRevisalManager**:
* Get the data from the previously generated file
* Register employee in REVISAL app* with the extracted data
* Handle two types of exceptions:  
a. when the CNP* is already entered in the system (employee is already registered)  
b. when the CNP is invalid (according to Romanian state standards)  

data* - First Name, Last Name and CNP  
CNP* - Romanian SSN  
REVISAL app* - Managing  employee app (see https://www.inspectiamuncii.ro/reges)  
