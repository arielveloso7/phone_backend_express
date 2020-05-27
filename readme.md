# PHONE BACKEND EXPRESS

### 1. Phonebook backend step1


Implement a Node application that returns a hardcoded list of phonebook entries from the address <http://localhost:3001/api/persons>:

![](./images/22e.png)


Notice that the forward slash in the route <i>api/persons</i> is not a special character, and is just like any other character in the string. 


The application must be started with the command _npm start_.


The application must also offer an _npm run dev_ command that will run the application and restart the server whenever changes are made and saved to a file in the source code.


#### 3.2: Phonebook backend step2


Implement a page at the address <http://localhost:3001/info> that looks roughly like this:

![](./images/23ea.png)


The page has to show the time that the request was received and how many entries are in the phonebook at the time of processing the request.


#### 3.3: Phonebook backend step3


Implement the functionality for displaying the information for a single phonebook entry. The url for getting the data for a person with the id 5 should be <http://localhost:3001/api/persons/5>


If an entry for the given id is not found, the server has to respond with the appropriate status code.


#### 3.4: Phonebook backend step4


Implement functionality that makes it possible to delete a single phonebook entry by making an HTTP DELETE request to the unique URL of that phonebook entry.


Test that your functionality works with either Postman or the Visual Studio Code REST client.


#### 3.5: Phonebook backend step5


Expand the backend so that new phonebook entries can be added by making HTTP POST requests to the address <http://localhost:3001/api/persons>.


Generate a new id for the phonebook entry with the [Math.random](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random) function. Use a big enough range for your random values so that the likelihood of creating duplicate id's is small.


#### 3.6: Phonebook backend step6




Implement error handling for creating new entries. The request is not allowed to succeed, if:
- The name or number is missing 
- The name already exists in the phonebook


Respond to requests like these with the appropriate status code, and also send back information that explains the reason for the error, e.g.:

```js
{ error: 'name must be unique' }
```

</div>

<div class="content">
