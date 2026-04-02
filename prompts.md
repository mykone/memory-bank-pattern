# First Prompt to LLama (Bad: no context)

"I have initialized the Memory Bank. According to TASKS.md, we are in Session 1. Please provide the commands to initialize the Go module and create the first PostgreSQL migration file for the users table."

# First Prompt to LLama (Better: Has context)
"Read these project files: @CLAUDE.md, @PROJECT.md, @ARCHITECTURE.md, @DATA_MODEL.md, and @TASKS.md.

Initialize Session 1. Based on the Architecture and Data Model documented in those files, provide the exact terminal commands to:

Initialize the Go module local-auth-pilot.

Install the necessary dependencies (gin, pgx, jwt, bcrypt).

Create the migration file structure (db/migrations/) and provide the SQL code for 001_create_users_table.sql based on the DATA_MODEL.md schema."

### Much Better Response
```sh
go mod init local-auth-pilot
go get gin@latest pgx@latest jwt@latest bcrypt@latest
mkdir -p db/migrations && touch db/migrations/001_create_users_table.sql
```