# Stand Alone Server


#### Initialize Project

* Run `npm install` inside the root directory of this project to install dependencies for the API server.
* Run `npm start` to start the API server.


####  Description

* Once your server is up and running, the URL you'll be able to hit from within your app is `http://localhost:5000`. You will however need an authentication header on all the calls except the login call.
* Take a look at the endpoints that our API has to offer in `server.js`.

  * **[POST]** * to `/api/login`: returns a token to be added to the header of all other requests. Pass in the following credentials as the `body` of the request: `{ username: 'lambda', password: 'school' }`
  * **[GET]** to `/api/yourData`: sub your data name returns the list of yourData.
  * **[GET]** to `/api/yourData/123`: sub your data with id returns the item with the id passed as part of the URL (123 in example).
  * **[POST]** to `/api/yourData`: creates a new entry and return the new list of items. Pass the friend as the `body` of the request (the second argument passed to `axios.post`).
  * **[PUT]** to `/api/yourData/:id`: updates the friend using the `id` passed as part of the URL. Send the an object with the updated information as the `body` of the request (the second argument passed to `axios.put`).
  * **[DELETE]** to `/api/yourData/123`: removes the friend using the `id` passed as part of the URL (123 in example).


