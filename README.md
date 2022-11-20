# learn-aspnetcore

Learn to create a web API with ASP.NET Core based [this tutorial](https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-7.0&tabs=visual-studio-code).

## Test Run Locally

1. <kbd>Ctrl</kbd> + <kbd>F5</kbd> or go to Menu -> Run -> Run Without Debugging
2. The browser should be automatically opened. Otherwise, grab the server URL and post from the debug console log.
3. Open the Swagger page at path `/swagger`.
4. Test the <kbd>POST</kbd> `/api/TodoItems` API with the following body:

    ```json
    {
      "name": "walk dog",
      "isComplete": true
    }
    ```

    You should get the following similar response:

    ```json
    {
      "id": 1,
      "name": "walk dog",
      "isComplete": true
    }
    ```

    The response's `location` header should point to the newly-created TodoItem:

    ```headers
    content-type: application/json; charset=utf-8 
    date: Sun,20 Nov 2022 08:35:35 GMT 
    location: http://localhost:5206/api/TodoItems/1 
    server: Kestrel 
    transfer-encoding: chunked 
    ```

5. Test the <kbd>GET</kbd> `/api/TodoItems/{id}` API for the new TodoItem an you should get the same response:

    ```json
    {
      "id": 1,
      "name": "walk dog",
      "isComplete": true
    }
    ```

6. Add another TodoItem with <kbd>POST</kbd> and test the <kbd>GET</kbd> `/api/TodoItems`.
7. Test the <kbd>PUT</kbd> `/api/TodoItems/{id}` by getting an item and update the data in the PUT request body.
8. Test the <kbd>DELETE</kbd> `/api/TodoItems/{id}` on an existing item.

_Note: You can also use [Postman](https://www.postman.com/), [curl](https://terminalcheatsheet.com/guides/curl-rest-api), or [httprepl](https://learn.microsoft.com/en-us/aspnet/core/web-api/http-repl/?view=aspnetcore-7.0) to test the APIs._