## Deployment

The Glue42 Server can be deployed on-premise and can run inside your organization network.

The deployment consists of the following:

- Glue42 Server - a NodeJS app, the actual server;
- Glue42 Server Admin UI - a React app that allows managing the data stored in the Glue42 Server;
- MongoDB database;

Docker images are available for the stock implementation. The Docker images allow you to deploy a stock version of the Glue42 Server.

If any customization is necessary, NPM packages exposing the Glue42 Server and the Glue42 Server Admin UI as modules are available. The modules provide extension points for different customizations like authentication and storage.

It is recommended to use the NPM packages as this approach is much more flexible.

### Using NPM Packages

#### Access

The NPM packages exposing the Glue42 Server and the Admin UI are hosted in a private NPM repository. To obtain access, [contact us](https://glue42.com/contacts/) at `info@glue42.com`.

#### Environment Setup

Generate an `.npmrc` file that will contain the authentication information for connecting to the private NPM repository. Make sure to exclude this file from your source control system.

To generate an `.npmrc` file:

- Login to [Glue42 JFROG](https://glue42.jfrog.io/).
- Expand the menu in top right.
- Click "Setup".
- Select "NPM".
- From the dropdown menu select `_default-npm-virtual_`.
- Copy the snippet.
- Create an `.npmrc` file with the copied contents.

#### MongoDB

The Glue42 Server uses [MongoDB](https://www.mongodb.com/) as a database. You must have a running MongoDB instance.

Now you can begin using the packages and start the server locally. For an example of how to run the Glue42 Server and the Admin UI using NPM packages and basic authentication, see the [Basic Server Example](https://github.com/Glue42/server-example-basic) repo on GitHub. Follow the instructions in the README file to start the Glue42 Server and the Admin UI.