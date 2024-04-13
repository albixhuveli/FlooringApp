# FlooringApp

Design Discussion

Individual Designs (Section A)

Design 1:
Con: Unnecessary function under employee.
Con: Login info for user is not needed as they are just users.
Con: Overlap of search functions.
Con: Missing material type.
Con: Water resistance missing from Vinyl and Laminate.
Con: The search goes directly to Floor, rather than to Category.

Pro: Incorporated some multiplicities.
Pro: the dual tone design of the UML allows for easy grasp of information.

Design 2
Con: Both employees and users get access to the same functions.
Con: The examples are specific, and shouldn’t be.
Con: Laminate and Vinyl can be resistant in boolean vs string.
Con: Size of floor is in String rather than a number.
Con: Store offering is repetitive.

Pro: Has various relevant association types.
Pro: Has a clear hierarchy.
Pro: Very detailed.

Design 3
Con: Store names are identical in a chain, so an ID is needed.

Pro: Neat, simple, and organized.
Pro: Clearly shows how the search works.
Pro: Shows good hierarchy.

Design 4
Con: Unnecessary database adds to UML complexion.
Con: Not the correct hierarchy.
Con: No customer needed, nor payment info as there is no purchasing in this store.
Con: Quantity size is not of the store, but rather of the individual floors.

Pro: Gave thought to the need of a database.






Team Design (Section B)

[embed pikshor]

Our main UML design uses a combination of both Design 2 and Design 3. We found this to be best, as Design 3 was oversimplified, it had the least cons, while Design 2 made up for it with the thorough details. All designs shared similarities in many aspects, such as making sure we have a user, employee, and floor types. Yet, the functions were different, as were some attributes.

We decided to share a direct relationship from user to store and from employee to store, as to have access to the offerings they need access to the store. This is in contrast to some of our other individual UMLs that didn’t account for a chain of stores. From there, we decided to tackle the hierarchy problem, making sure that after store we have the various products, and from there we have the categories (first level) and floor types (second level). So to search, we made sure to combine all the search functions under the User, as they will be the ones searching for floors. 

In order to include employees, we have a login function that uses an employees ID and PIN number. We also decided to assign StoreID to employees so we can make sure their edited products are at their own stores.


Summary (Section C)

We elaborated on how to make each other’s design better. We compared and implemented each of our designs to one and the pros and cons helped us determine what to exclude and include in the design. We considered flexibility in our design while making it, since there are many interpretations of a request for a design. Having a team that criticizes each one’s interpretation, we can create an optimum design to satisfy the request. 
















April 3rd Inc.

ToDo:
Project plan (ProjectPlan.md), showing roles and phases (see template).
Use-case model (UseCaseModel.md) (see template).
Supplementary requirements (i.e., requirements that do not fit the use-case model, such as non-functional requirements). These can be provided as a simple list. Put this in an MD file called ExtraRequirements.md
Design document (DesignDocument.md) (see template).
Test plan without results (TestPlan.md) (see template).





Project Plan

**Author**: Team 5: Liza Hashani, Tanvir Sami, Albi Xhuveli

##  1 Introduction

Our app makes it simple and easy to search and track inventory of flooring products for each store in Flooring Icon Inc.


## 2 Process Description

As a team we will use the phases of the software development life cycle in the process of creating our application. We produce the concepts and analyze the requirements needed. We form architectural and detailed designs of both internal and external structure as well as thoroughly planning their functionality. Lastly we implement code, debug, and test our final result.

**Inception**
- The team makes note of the requirements from the owners. We analyzed the specifications, and established clear goals for each process to be completed in order to have a working design and functionality.
- The entrance criteria for this phase are the concepts and requirements analysis. We also plan out development and correction costs, analyze any risk factors, and design general architectures of the software.
- The exit criteria for this phase consists of all the documents forming our software concepts and scope such as a project plan, use-case model, risk assessments, and business case. 

**Elaboration**
- In the elaboration phase we use our previous documentation to further design a more detailed outline and elaborate on supplementary requirements, dependencies, and operations. Multiple diagrams are created to organize the software’s components and deployment with detailed documentation. We check that these all meet the requirements.
- The entrance criteria of this phase is all that is described above.
- The exit criteria here is having solid design models for the UI, hardware and software structures, as well as all test cases prepared.

**Construction**
- In the construction phase all team members will use the architectural designs from our elaboration to begin the code implementation and building the interface. We develop all features within the working system with all the functional and technical requirements. All the functional requirements are tested.
- The entrance criteria of this phase are the above details. The prototype, or initial version of the app, should be executed. Requirements can be refined as well.
- The exit criteria for this phase is that the software application is completed and functions as needed on the android device. A user manual should also be constructed and finalized. All testing strategies are performed with available results. 

**Transition**
- In the transition phase, we catch any software issues or bugs. This is when beta testing will be performed, meaning it will be tested and validated by users/employees. We want to ensure that the app is user-friendly, functional, and efficient. 
- The entrance criteria for this phase is the final version of the application. Final edits are made to the documentation. The improved tests should provide final and successful results.
- The exit criteria is that our Flooring Inc application is completed and can be used.


## 3 Team

Team members: Liza Hashani, Tanvir Sami, Albi Xhuveli
Table of Roles™

| Team Member       | Role        |
| -----------       | ----------- |
| Liza Hashani     | Project Manager  / Frontend dev (main), Backend dev(sub), QA lead   |
| Tanvir Sami | Backend dev (main), Frontend dev (sub), QA tester   |
| Albi Xhuveli | Backend dev (main), Frontend dev (sub), QA tester  |
















Use Case Model

# Use Case Model

**Author**: Team 5: Liza Hashani, Tanvir Sami, Albi Xhuveli

## 1 Use Case Diagram















## 2 Use Case Descriptions

### Search Product Name
**Requirement:** Allows user/employee to directly search a product by its name
**Pre-conditions:** Open app and select whether you are a user or an employee
**Post-conditions:** User/employee can search for a product by its name
**Scenarios:** A user wants to search for a product by name
An employee wants to search for a product by name

### Select Category
**Requirement:** Allows the user/employee to select a floor category from the given options on the home screen.
**Pre-conditions:** A user must go through the user option in the home screen. An employee must go through the authentication process from the home screen to search categories.
**Post-conditions:** user/employee can search for a product by its category. 
**Scenarios:** A user/employee wants to search for a product by category.

### View Product
**Requirement:** Allows the user/employee to view expanded details on the selected  product such as category, detail, and store quantity.
**Pre-conditions:** user/employee must search for the product and have the product in list form to select it. 
**Post-conditions:** The product detail will be displayed including the category, detail, and store quantity.
**Scenarios:** A user/employee wants to view more information on a product.

### Authenticate
**Requirement:** Allows the Employee to manipulate product details.
**Pre-conditions:** Employees must open the app and login using their pin
**Post-conditions:** Employee is now verified and has access to manage inventory
**Scenarios:** An employee wants to use the app to make changes to a product. They log in first to verify that they’re an employee and can make the changes.

### Add Product
**Requirement:** Allows the Employee to add products
**Pre-conditions:** An Employee must open the app, login with their pin, and finally add a product.
**Post-conditions:** A product has been added to the listing by an Employee.
**Scenarios:** An employee wants to update the inventory by adding a product.

### Delete Product
**Requirement:** Allows the Employee to delete products 
**Pre-conditions:** An existing product listing must be available to be deleted by an employee. The employee must also be logged in using their pin to see the option to delete a listing.
**Post-conditions:** The listing is deleted from the inventory.
**Scenarios:** A product is removed from the store and needs to be deleted from the app.


### Edit Product
**Requirements:** This will allow the employee to edit a product’s details.
**Pre-conditions:** An existing product listing must be available to be edited for an employee to edit it. The employee must also be logged in with their pin to see the option to edit a listing.
**Post-conditions:** Employees are able to edit the existing details of a product.
**Scenarios:** The employee is interested in editing the details of an item due to a mistake or an update in stock.



### Select Store
**Requirements:** Allows user to check at which store the product is available at
**Pre-conditions:** User must select a product in order to view its details and availability
**Post-conditions:** User can check the availability of the product
**Scenarios:** A user selects an item and wants to view more details about it in a specific store, such as quantity in stock.


# Supplementary Requirements

- **Aesthetically Pleasing:** The application should be simple to use and organized, giving the application personality and therefore making it likable. We want the user to be able to find what they need quickly and easily.
- **Availability:** The application must always retrieve the data related to a specific user, making the application useful at all times.
- **Efficient Performance:** The application must be quick in returning and displaying data to the user.
- **Scalable:** The application must allow the employee to be able to add as many floors as needed.
- **Reliability and compatibility:** The application must perform without any crashes or freezes. 
- **Serviceability:** A user should be able to view all products in the app and employees should be given access to add, delete and edit products of their store. 
- **Usability:** The application must be user-friendly and employee-intuitive. Ideally, it can be picked up by anyone very quickly, intuitive and self-explanatory.


































Design Document

# Design Document

**Author**: Team 5: Liza Hashani, Tanvir Sami, Albi Xhuveli

## 1 Design Considerations

### 1.1 Assumptions

This app will be used by both employees and guest users
Users will look at various stores for quantity
Each floor only has one corresponding floor category
Product availability is dependent on updated information given by employees

### 1.2 Constraints

Time: This application must be completed before the end of the semester if not before.
Layout: The application must be adaptable to a standard smartphone screen size. The fonts of icons and search words, as well as the language must be consistent. 
Latency: The application will have to instantly respond and load page information and images to make it convenient for the users.
Testing: Application must successfully pass all test cases after design and implementation is complete.

### 1.3 System Environment

Android operating system with minimum API of 21.

## 2 Architectural Design 

### 2.1 Component Diagram

	The main components that will be working together are 
The User component, The Employee component, UI component, and Product Database component.
The main interaction is happening between the user/employee and the store UI where the user/employee can search for an existing item in  the flooring list.
Adding and deleting a product can also be completed by the employee. 




### 2.2 Deployment Diagram

The application’s deployment consists of the android UI as the main device in connection with the store as the main component. This is in direct connection with the product database as our server. In terms of clients, our users access only the UI and employees have access to product management in the database through authentication. Our application is a simple system because it relays data to only one database, and in terms of hardware the users and employees have direct access to the physical means of the application.


















## 3 Low-Level Design

### 3.1 Class Diagram


### 3.2 Other Diagrams


## 4 User Interface Design





























Test Plan

# Test Plan

**Author**: Team 5: Liza Hashani, Tanvir Sami, Albi Xhuveli

## 1 Testing Strategy

### 1.1 Overall strategy

*This section should provide details about your unit-, integration-, system-, and regression-testing strategies. In particular, it should discuss which activities you will perform as part of your testing process, and who will perform such activities.*

Our overall testing strategy is to check if the system is able to provide the users or employees with their desired data. Our unit and integration testing will mainly be done by our backend developers and the functional testing by our frontend developers. The goal is to have the most unit tests and less integration tests. We will use the method of regression testing after every change is made to a component to make sure everything functions as it should. Some examples include that we need to test conditions where a user/employee searches for a product that is not available or does not exist. We also need to check if a product edited by an employee has been updated for the user in real time, so there isn’t any misinformation.    

### 1.2 Test Selection

*Here you should discuss how you are going to select your test cases, that is, which black-box and/or white-box techniques you will use. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*

In order to test the previous strategies, we will use both black box and white box techniques. We can use black box testing to test the external functions of the app as it is a simple program and any visual error we find on the app can be assumed in the codes. These errors can include errors such as wrong product quantity displayed in a store, or a product that has been edited but not updated in the search. This may also include any distorted screen pages or icons. We can also utilize white box techniques by implementing inputs to check and verify loops and conditions. We will also conduct a form of path testing by executing every possible independent path that source code may take, this way we can pinpoint all faults within the code.

### 1.3 Adequacy Criterion

*Define how you are going to assess the quality of your test cases. Typically, this involves some form of functional or structural coverage. If you plan to use different techniques at different testing levels (e.g., unit and system), you should clarify that.*

We will assess the quality of our test cases by quantity. We will repeat 
our tests many times with multiple conditions and make changes to them when necessary in order to have minimum bugs in our code. To ensure that each component is being tested, there will be a test for each activity in the application’s functional process such as the login authentication, viewing of products, editing abilities, and so on. The team developers who have knowledge about the internal structure (code) of this program will conduct the main logical testing. It is important that they communicate their findings with those who conduct external testing as well to better the testing techniques. 
 
### 1.4 Bug Tracking

*Describe how bugs and enhancement requests will be tracked.*

Our team will need a program that monitors the source code and incorporates a bug tracking database that contains the information of any known bugs found. If the program detects a bug in the app, the user will have the option to report the bug. Any reported bugs will be saved as well as enhancement requests. Enhancement requests can be made by contacting the app developer.

### 1.5 Technology

*Describe any testing technology you intend to use or build (e.g., JUnit, Selenium).*

The program will be tested by executing the Junit technology test cases.


## 2 Test Cases

*This section should be the core of this document. You should provide a table of test cases, one per row. For each test case, the table should provide its purpose, the steps necessary to perform the test, the expected result, the actual result (to be filled later), pass/fail information (to be filled later), and any additional information you think is relevant.*

These test cases were done to test the individual functionality of the activities and functions and their connectivity to each other.


ACTIVITIES:
- ProductDescriptionActivity
- DeleteItemActivity
- EditProductActivity
- MainActivity
- LoginActivity
- ProductListActivity
- CategoryActivity
- SearchProductActivity

We will describe below the activities the app will be used for to ensure that we will test each one for any bugs.

1. Logging into the app.
2. Searching for a product in the database.
3. Editing a product.
2. Deleting a product from the database.
3. Adding a product to the database.
4. Selecting a category.
5. Selecting a product.
6. Selecting a store from the product dropdown.
7. Editing the quantity of a previously added product.
8. Renaming a previously added product.
9. Editing the color of a previously added product.
10. Editing the category of a previously added product.
11. Editing the correct store listing of the employee.
16. Displaying an error at the employees when attempting to enter empty values.

|Test Case Description|Activity|Steps|Expected Result|Actual Result |Pass/Fail|
|---------------------|---------|-----|---------------|-------------|------|
|Start the App|None|Install and open the App|The app would run successfully and would show the Main Activity screen.|||
|Log into the app|MainActivity|Open the app and click login, then put in the credentials|The app should authenticate and if the credentials are correct show the category screen (CategoryActivity) with the correct buttons|||
|Editing the product description|EditProductActivity|Once logged in, click on a category. Secondly, click on a product. Then, click on the edit button and edit a detail. Finally, click confirm.|The app should update the product listing and bring you back to the updated product the employee just edited|||
|Searching for a product by name|SearchProductActivity|From the main screen, click the search bar. Then, type a name in.|The app should display all the product listings with that name.|||
|Selecting a category from the category page|CategoryActivity|From the main screen, click a category.|The app should display all the product listings of that category type.|||
|Selecting a product from the floor product list using categories|ProductDescriptionActivity|From the main screen, click a category. Then, click on a product listing.|The app should display the product details.|||
|Selecting a product from the floor product list using categories|ProductListActivity|From the main screen, click a category. Then, click on a product listing.|The app should display the product details.|||
|Selecting a product from the floor product list using search|ProductListActivity|From the main screen, click the search bar. Then, type a name. Finally, click on a product listing.|The app should display the product details.|||
|Selecting a store from the product dropdown.|ProductDescriptionActivity|Click a product list. Then, click on the store dropdown and select a store.|The app should display the product details for the selected store.|
|Renaming a previously added product.|EditProductActivity|Click a product list. Then, click the edit button. Finally, change the name of the product and click confirm.|The app should display the product details for the selected store with the changed name.|||
|Editing the color of a previously added product. |EditProductActivity|Click a product list. Then, click the edit button. Finally, change the color of the store and click confirm.|The app should display the product details for the selected store with the changed name.|||
|Displaying an error at the employees when attempting to enter empty values.|EditProductActivity|Click a product list. Then, click the edit button. Finally, remove the name of the product listing and click confirm.|The app should display an error message with the option to confirm|||
|Clicking on confirm of an error message brings you back to the original page|EditProductActivity|Click a product list. Then, click the edit button. Remove the name of the product listing and click confirm. Then, click confirm on the error popup.|The app should return to the product editing screen|||































# User Manual 

## The User Manual for Flooring Icon Inc.





The homescreen of the app.



By clicking this button you will be able to view and search for available products in the store.








After clicking on explore you can view the different categories of flooring available through the images shown.


#### How to use Search


Users/employees both can search for products by typing out the name.












### How To Register As An Employee

This button allows you to register as an Employee.



On this screen you may register as an employee by inputting your email, store id, and creating a password. Then after clicking register you will be added as an employee to the database.



Employees can register by entering their email address here.



Employees can create a password with their registration.
 

Employees can specify which store they are registering for.





#### How To Login As An Employee


The employee login screen is shown.
Here you are able to login to make changes to the database by adding products, editing, or deleting them.



Employees can enter the registered email here.



Employees can enter the registered password here.



If you are not an employee, you can click on this button to redirect you back to the search page of the app.


### How To Add Items As An Employee


After logging in as an employee and clicking on “All Floors” you can select the Add New Item button.



This is the Add New Item screen.
You can use this screen to add a new flooring product and specify the name, category, square footage, and to which store the product belongs to.



The name you want to label the flooring as can be input under “Floor Name.”



The arrow pointing down can be clicked on the category bar to select which category you want to put the new item under.



These are the 5 available categories you can choose to add an item.


Here you input the floor type for the item 

Here you select the amount of square footage a new item has.



Here you input the store ID you will be assigning a new item to.


Here you input the size of the product you will be adding. *****


Here you will be selecting the color of the item you will be adding.


Here you input the price of the item you will be adding.


Under “Brand” you can specify the brand name of the product you are adding.






Here you can specify the Material of the floor (tile, porcelain, marble, slate, etc).


Here you can specify the species of only the Wood floors.


This option is only available for types Laminate and Vinyl. Specify whether the product is water resistant by enabling it or disabling it.




When adding a Vinyl Floor if you do not enable Water Resistance, it classifies the floor as its alternative, which is Waterproof. Specify whether the product is water resistant/waterproof by enabling it or disabling it. 


As for Laminate, if you do not enable Water Resistance, it classifies the floor as its alternative, which is Regular Laminate.

After you have specified all the required information for the product you wish to add, select the checkmark to add the new item to the database.








































### How to Log Out As An Employee.



After clicking “Begin Exploring Here” you will be led to this search page, if you wish to logout and go back to the home screen then scroll all the way down and click on the logout button.

















### Viewing All Floors Inventory Catalog (User & Employee)


In order to view all floors that the chain offers as a user, click on “Begin Exploring Here.” If you are an employee, register/sign in first.



You will be directed to the Category page, and you select which store you would like to view all floors available. 





Click on the drop down menu that says “Select Store ID to search from:” Select the store ID of the store you wish to see the products for.




Select “All Floors.”








You can see the Floors along with its category, color, brand, and price that is available for the selected store.


After selecting a single product, you will be able to see further information as shown above, such as the type, size, species, or whether it's waterproof or water resistant.




















###How To Edit/Delete A Product




If you are signed in as an employee at this point, you can select the left icon to edit the information of that product or the right icon to delete the product.  


If you select to edit an item you will be directed to this page where you can change details about the item. Once you have finished changing then you can press the check mark on the bottom right hand corner to save and exit the edit item page.





|Test Case Description|Activity|Steps|Expected Result|Actual Result |Pass/Fail|
|---------------------|---------|-----|---------------|-------------|------|
|Start the App|None|Install and open the App|The app would run successfully and would show the Main Activity screen.|The app opened a home page |pass|

|Log into the app|MainActivity|Open the app and click login, then put in the credentials|The app should authenticate and if the credentials are correct show the category screen (CategoryActivity) with the correct buttons|The app displayed the categories after logging in with credentials|pass|

|Editing the product description|EditProductActivity|Once logged in, click on a category. Secondly, click on a product. Then, click on the edit button and edit a detail. Finally, click confirm.|The app should update the product listing and bring you back to the updated product the employee just edited|The app updated the details as per edit|pass|

|Searching for a product by name|SearchProductActivity|From the main screen, click the search bar. Then, type a name in.|The app should display all the product listings with that name.|The app displayed the results with the correct query|pass|

|Selecting a category from the category page|CategoryActivity|From the main screen, click a category.|The app should display all the product listings of that category type.|The app displays the results related to the category selected|pass|

|Selecting a product from the floor product list using categories|ProductDescriptionActivity|From the main screen, click a category. Then, click on a product listing.|The app should display the product details.|The app displays the corresponding product details|pass|

|Selecting a product from the floor product list using categories|ProductListActivity|From the main screen, click a category. Then, click on a product listing.|The app should display the product details.|||

|Selecting a product from the floor product list using search|ProductListActivity|From the main screen, click the search bar. Then, type a name. Finally, click on a product listing.|The app should display the product details.|||

|Selecting a store from the product dropdown.|ProductDescriptionActivity|Click a product list. Then, click on the store dropdown and select a store.|The app should display the product details for the selected store.|
|Renaming a previously added product.|EditProductActivity|Click a product list. Then, click the edit button. Finally, change the name of the product and click confirm.|The app should display the product details for the selected store with the changed name.|||
|Editing the color of a previously added product. |EditProductActivity|Click a product list. Then, click the edit button. Finally, change the color of the store and click confirm.|The app should display the product details for the selected store with the changed name.|||
|Displaying an error at the employees when attempting to enter empty values.|EditProductActivity|Click a product list. Then, click the edit button. Finally, remove the name of the product listing and click confirm.|The app should display an error message with the option to confirm|||
|Clicking on confirm of an error message brings you back to the original page|EditProductActivity|Click a product list. Then, click the edit button. Remove the name of the product listing and click confirm. Then, click confirm on the error popup.|The app should return to the product editing screen|||
