ASSUMPTIONS:
1. Public API returns limited quantity data
2. Private API returns all data
3. Methods create, delete only for private API because the only User with privileges can manipulate with data
4. Inserting several users are developed via an array 
5. Parameter 'Desired salary' only for private API because only authorized request can get information about private information
6. Methods delete and delayed response won't be involved due to specific tasks
7. Parameters age, gender can be null
8. Parameter desired salary is not null
9. Password generated via specific method and won't be involved in task 2

1 - Login through Public API for getting Token
2 - Login through Public API for getting Token and error 401 due to a problem with the client’s credentials
3 - Login through Public API for getting Token and error 403 due to a problem with access, User doesn't have access for getting Token
Task 1:
4 - Request through Private API for getting All Users with Token and getting a all users data
5 - Request through Private API for getting All Users with Token and getting error 500 in the case when Server has down
6 - Request through Public API for getting All Users with Token getting error 404 in the case when request incorrect

Task 2:
7 - Request for creating new Users through Private API
8 - Request for creating new Users through Private API and getting error 422 with incorrect values in parameters 
9 - Request for creating new Users through Private API and getting error 400 with Invalid JSON data in request body: Syntax error.

Task 3:
10 - Request for searcing users with desired salary less then 100.000 and use the search feature from Elascticsearch
11 - Request for searcing users with desired salary less then 100.000 and getting error 405 due to server has rejected that particular method for the requested resource