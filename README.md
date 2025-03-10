GraphQL Server
About the Project:
This GraphQL project demonstrates how to set up a basic server using Node.js and GraphQL for querying and mutating data. It is designed to provide a starting point for building more complex GraphQL applications. The project includes server setup, schema definition, and basic data handling with a focus on integrating GraphQL queries, mutations, and resolvers.

Features
✅ Set up of a basic GraphQL server with Node.js
✅ Define GraphQL schema using typeDefs and resolvers
✅ Support for basic queries and mutations
✅ Integration with a simple database (e.g., local file or in-memory data)
✅ Express.js middleware for GraphQL server

Technologies Used
Node.js - JavaScript runtime for backend development
GraphQL - Query language for APIs
Express.js - Web application framework for Node.js
Apollo Server - A popular GraphQL server implementation
MongoDB or In-memory data - For storing and retrieving data
npm - Dependency management

Project Structure
/GraphQL
│── /server
│   ├── db.js              # Database connection or in-memory data setup
│   ├── schema.js          # GraphQL schema definition (queries, mutations, types)
│   ├── server.js          # Express server setup and GraphQL endpoint configuration
│── node_modules           # Project dependencies
│── .gitignore             # Git ignore settings
│── package.json           # Project dependencies and scripts
│── package-lock.json      # Lock file for project dependencies

Installation & Setup
1.Clone the repository:
git clone https://github.com/saraswathi2015/GraphQL.git

2.Navigate into the project directory:
cd GraphQL

3.Install dependencies:
npm install

4.To start the GraphQL server:
node server/server.js
The GraphQL server will be available at http://localhost:4000/

Usage
Open the GraphQL server in a browser or GraphQL Playground tool to interact with the API.

You can execute queries like:
Example Query:
{
  getUsers {
    id
    name
    email
  }
}
Example Mutation:
mutation {
  createUser(name: "John Doe", email: "john@example.com") {
    id
    name
  }
}
The server responds with the requested data based on the GraphQL schema you define.
