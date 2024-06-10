# Tutorial: Edit recipient info

In this tutorial, you'll learn how to edit the information for a recipient.

Expect this tutorial to take about 15 minutes to complete.

## Edit a recipient

Adding a recipient to the service requires that you add (`POST`) the details of a new [`recipient`](../api/create_recipient) resource to the service.

To add a recipient:

1. Make sure your local service is running, or start it by using this command, if it's not.

    ```shell
    cd <your-github-workspace>/gift-lookup-service/api
    json-server -w gift-lookup-db-source.json
    ```

1. Open the Postman app on your desktop.
1. In the Postman app, create a new request with these values:

    * **METHOD**: POST
    * **URL**: `{{base_url}}/recipients`
    * **Headers**:`Content-Type: application/json`
    * **Request body**:
        You can change the values of each property as you'd like.

        ```js
        {
        "last_name": "Vaz",
        "first_name": "Elizabeth",
        "date_of_birth": "2020-04-14"
        }
        ```

1. In the Postman app, choose **Send** to make the request.
1. Watch for the response body, which should look something like this. Note that the names should be the same as you used in your **Request body** and the response should include the new recipient's `id`.

    ```js
    {
        {
        "last_name": "Vaz",
        "first_name": "Elizabeth",
        "date_of_birth": "2020-04-14",
        "id": 1
        }
    }
    ```

After doing this tutorial in Postman, you might like to repeat it in your favorite programming language. To do this, adapt the values from the tutorial to the properties and arguments that the language uses to make REST API calls.

## Next steps

TBD

## Related information

* [Handling errors](handling_errors.md)
