# UltraAutomationAPI
## That Automation collection running using for testing the below requests: 
 1. Create User
 2. Update User
 3. Deleted

## PreRequiste:
* Install newman
* Register in the gorest app to get the bearer token authentcication then set it as a global variable
* insert the data for testing as env variable in env variable file (Enter your new data everytime for your run)
_________

## Request Tests
## Every request hast its own tests written in JS 

### Create User Tests:
  * Verify that the name exists in the response body
  * Verify Status code is 201
 
### Update User Tests:
 * Verify that the name is updated in the response body
 * Verify that the email is updated in the response body
 * Verify Status code is 200

### Delete User Tests:
 * Verify Status code is 204
_________


## Run Tests

### Run the collection from Postman:
  * Right click on the collection then select (run collection)

###
![image](https://user-images.githubusercontent.com/66884373/131122694-2ae44f17-645b-4020-a0a9-5cbd4ed49309.png)

### Run the collection from the command:
  * Install newman using the below command
 ```bash 
  $ npm install -g newman
  ```

  * Right click on the collection then select (run collection)
  ```bash 
   newman run {{collectiionName}}.json -e {{envVariableName}} -g {{globalVariableName}}
  ```










