# Testing Trello REST API using Postman

These are API tests for Trello conducted using Postman. <br>

Trello is a web-based project management tool that allows users to organize tasks and workflows using a visual interface with boards, lists, and cards. It is designed to enhance productivity and collaboration among team members.<br>

Postman is a popular API development tool used to design, test, and debug APIs. It offers features such as API documentation, automated testing, and collaboration among team members. Postman supports multiple HTTP request methods and allows developers to send requests to a server and receive responses. <br><br>

## Test scope

The test focus is on the Boards module from the Trello API documentation. <br>
These are functional and unit tests checking the operation of the following **CRUD operations**: <br>
* POST 
  - Create a board with a valid name
  - Create a board with no name
  - Create a board with a name that consists of only a space or spaces
  - Create a board with a name that consists of special characters

* GET 
  - Get a board
  - Get all boards

* PUT 
  - Update the name of the board to the correct new name value
  - Update the board name to consist of only one space or multiple spaces
  - Update the name of the board to include no name value
  - Update the name of the board to include special characters
  
* DELETE
  - Delete a board <br><br>

Test were conducted based on a <b>test scenario</b>: ![testScenario_TrelloAPI.pdf](./testScenario_TrelloAPI.pdf)<br>

**Bug report**: ![bugReport_TrelloAPI.pdf](./bugReport_01_TrelloAPI.pdf)<br>

⚡🤖 During the testing procedure, **28 automated tests** were executed. 🤖⚡ <br>

The complete Trello REST API documentation is available [here](https://developer.atlassian.com/cloud/trello/rest/). <br><br>

## Getting started
### Postman installation
* Go to [the Postman website](https://www.postman.com/downloads/) and click the download button.
* Once the download is complete, run the installer and follow the on-screen instructions.
* After installation, Postman is ready to use for API development and testing.

### Authentication
#### To generate a token and API key in Trello:
* Log in to your [Trello](https://trello.com/) account.
* Go to the Trello developer [API key generation page](https://trello.com/app-key).
* Click on the "Go to the Power-Up Admin Portal", then click "Create New Key" button and enter the required details.
* Your API key will be displayed on the page. Copy and save it for use in API requests.
* Next, click on the "Token" link next to your application name.
* Authorize your application to access your Trello account.
* Your token will be displayed on the page. Copy and save it for use in API requests.

#### To save your Trello API key and token as environment variables:
* Open Postman and click on the "Environment" dropdown in the top left corner.
* Click on the "New" button to create a new environment and choose "Environment" icon.
* Give your environment a name and add the Trello API key and token as key-value pairs. <b>NOTE! For collections from this repository, the API Key variable is named {{APIKey}} and the token variable is named {{token}}.</b>
* Click "Save" to save the environment.
* In your request, click on the "Environment" dropdown and select the environment you just created.
* Use the {{Variable}} syntax in your request to reference the environment variables. <br><br>

## Run locally
* Clone the repository on your computer using the command: `git clone https://github.com/paulinaszybinska/Trello-REST-API.git`
* Run Postman and click on "Import" in the top left corner.
* Drag and drop the files "File name" from the cloned repository folder into the "Import" window.
* Choose to import your API as a Postman Collection or as OpenAPI 3.0 with a Postman Collection
* The collection will be downloaded and saved in Postman, ready for use. <br><br>

## Collection and Testing
To run the entire collection and perform a full loop of automated tests:
* Log in to Postman.
* Click on the "Collections" icon.
* From the list of collections, select the one named "The Trello REST API" and click on the icon with three dots that appears when you hover over the collection name.
* Select "Run collection".
* Click one the "Run The Trello REST API". 

After completing these steps, you will receive a full report on the status of HTTP requests and the accompanying test results. <br>
There is a similar option to separately run individual folders that make up the collection. <br><br>

## Author
Paulina Szybińska - [LinkedIn profile](https://www.linkedin.com/in/paulina-szybinska/) <br><br>

## 🍒🍒🍒 Appreciation 🍒🍒🍒
This project was created during the COLT 1/2023 initiative, led by the amazing [Ania Czyrko](https://www.linkedin.com/in/ania-czyrko-05933aa1/), the author of [Cherry-it blog](http://cherry-it.pl/). Thank you for the vast knowledge and patience you put into helping people who are starting their adventure with the world of testing! Big up! <br><br><br>

