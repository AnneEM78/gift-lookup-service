# Tutorial: Add a gift

In this tutorial, you'll learn how to add a new gift.

Expect this tutorial to take about 15 minutes to complete.

## Add a gift

Adding a gift to the service requires that you add (`POST`) the details of a new [`gift`](../api/create_gift.md) resource to the service.

To add a gift:

1. Make sure your local service is running, or start it by using this command, if it's not.

    ```shell
    cd <your-github-workspace>/gift-lookup-service/api
    json-server -w gift-lookup-db-source.json
    ```

1. Open the Postman app on your desktop.
1. In the Postman app, create a new request with these values:

    * **METHOD**: POST
    * **URL**: `{{base_url}}/gifts`
    * **Headers**:`Content-Type: application/json`
    * **Request body**:
        You can change the values of each property as you'd like.

    ```js
    {
      "user_id": 1,
      "title": "Gabby's Dollhouse",
      "date_gifted": "2024-02-20",
     }
        ```

1. In the Postman app, choose **Send** to make the request.
1. Watch for the response body, which should look something like this. Note that the gift title should be the same as you used in your **Request body** and the response should include the new gift `id`.

    ```js
    {
        {
      "user_id": 1,
      "title": "Gabby's Dollhouse",
      "date_gifted": "2024-02-20",
      "gift_id": 1
    }
    }
    ```

After doing this tutorial in Postman, you might like to repeat it in your favorite programming language. To do this, adapt the values from the tutorial to the properties and arguments that the language uses to make REST API calls.

## Next steps

TBD

## Related information

* [Handling errors](handling_errors.md)
