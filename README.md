# nodejs-api-test


## Testing RESTful API via Postman
1. After running MongoDB and server.js, open postman and onput http://localhost:3000/tasks in the request URL with GET method.
After sending, you should see “[]” because there is nothing in the database yet.

2. On the same address, change the method to POST, click body and select “x-www-form-urlencoded”.<br/>
Then, enter name as the key and the corresponding task name as value.<br/>
Click on send button. <br/>
This should give you a response 200 ok. <br/>
After that, you should read the data using GET method.

3. To delete task, change to DELETE method and url to http://localhost:3000/tasks/taskid.<br/>
After that, you can use GET method to check using the same url.

4. If we entered a wrong route like 'http://localhost:3000/abc', <br/>
it responds with a 404 status and show "url": "/ not found". 
