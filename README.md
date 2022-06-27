# [Kuehne+Nagel] Technical task for a backend developer

Write a NodeJS-based solution in JavaScript, using Express framework and ES6 language features.
1. The solution should provide REST API which accepts  "from" and "to" date as input parameters.
2. Then solution, upon request to it's rest interface, should asynchronously read data from a table in database (can be mocked) an array of objects with fields "id", "code", "name", "date"
3. Filter acquired data with all of the following rules (logical AND):
   - "id" field is not null, empty or undefined
   - "code" strictly equal to string "025"
   - "name" contains text "test"
   - "date" is between "from" and "to" values, which were obtained in the step 1

4.Then the solution should take this  objects and send it to a function which "simulates" another REST service. This function should group the received data and count unique id's per year (objects with fields: "year", "quantity"). 
5.Result of this function should be returned as response to the initial request.

The solution interface must comply with the REST standard.
 
Optional: 
Write a Docker file to run solution in Docker environment
Create tests(you can use any library)


Good luck!
