# Architecture
- **Language:** Go 1.23+ (Gin Framework)
- **DB:** PostgreSQL
- **Tools:** sqlc, migrate, bcrypt

## File Tree
├── main.go
├── db/
│   ├── queries/
│   ├── migrations/
│   └── sqlc/ (Generated)
├── handlers/
└── config/