# Itsajoke
Download the postgresql on the local system.
Go to terminal. Type `brew install postgresql`.
After the installation, you can start the postgres with `brew services start postgresql`. To stop we use command `brew services stop postgresql`.
To run postgres use command `psql postgres`.

We can use the default database `postgres`. To make connection, use the command`\c postgres`.
Create a relation called joke
`CREATE TABLE joke(
    id SERIAL PRIMARY KEY,
    setup VARCHAR(1000),
    punchline VARCHAR(1000),
    type VARCHAR(255)
);`

In backend folder, uncomment function importJokesIntoDB() and run it to import the data into the db ; 

Now goto the backend folder, type "cd backend". Once youre in the backend folder, run "npm i" to install the packages.
start backend server with "node server.js"
open index.html file using the local server.
