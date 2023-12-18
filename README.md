# Hub88 Developer Challenge

As a Hub88 developer, you will be interacting directly with the Hub88 APIs, the *"Game Providers APIs"* and the *"Operators APIs"*.

An "Operator" needs to implement the API defined by the [Operator Documentation](https://hub88.io/docs/operator) to handle received requests from Game providers via Hub88.

**To test your skills, you need to develop your own Operator's _"Wallet API"_ service implementation for the following endpoints**

#### `/user/balance`
- user's balance should be returned.
- If user doesn't exist in the system, this endpoint should create new user with balance of `1000` in `EUR` currency.
#### `/transaction/bet`
- user's balance should be decreased by the given `amount`.
- request should be validated properly, before processing it.
- Appropriate error should be returned incase of invalid requests.
#### `/transaction/win`
- user's balance should be increased by the given `amount`
- win request should have valid bet transaction(`reference_transaction_uuid`)
- Appropriate error should be returned incase of invalid requests

### Please be strict to the following development guidelines:
- Keep it simple;
- Should be written in Elixir [Phoenix framework](https://hexdocs.pm/phoenix/overview.html);
- You can choose database, dependencies on your preference;
- Do **NOT** implement the request's "signature" requirements;
- Authentication is not mandatory. But would be nice to have [Basic Authentication](https://swagger.io/docs/specification/2-0/authentication/basic-authentication/) for those endpoints;
- Implement the transactions endpoints properly, including corner-cases;
- Transaction should be idempotent. meaning that the same transaction cannot be processed multiple times;
- Ensure that your source code is clean and readable;
- Your code must be on GitHub as a private repository. Send an invite to [@segaz2002 and @gokul-poongodi](https://github.com/segaz2002, https://github.com/gokul-poongodi)

**Note:** There are no explicit deadlines. However, do note that proceeding with your challenge is subject to the availability of the position.
Keep in touch with the recruitment contact to plan your delivery.

After sharing your project, we will schedule your presentation/evaluation meeting.

### Please be strict to the following presentation guidelines:
- Keep it simple;
- Start by performing a live demo of your solution;
- Finally, explain how your API works while showing the project's source code in an editor/IDE of your choice;
- Be ready to answer technical questions related to your project.

For further clarifications, be in touch with the recruitment contact.
