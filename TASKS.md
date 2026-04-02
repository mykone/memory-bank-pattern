# Roadmap

## Session 1: Environment & Schema [⏰]
- [✅] Create CONTRACT.md
- [ ] Initialize Go mod.
- [ ] Create SQL migration for users table.
- [ ] Configure sqlc.yaml and generate boilerplate.

## Session 2: Auth Logic
- [ ] Create `password_utils.go` (Bcrypt).
- [ ] Create User repository in `db/sqlc`.

## Session 3: API Handlers
- [ ] Create `LoginHandler` in Gin.
- [ ] Implement request binding (email/password).

## Session 4: Main & Database Connection
- [ ] Setup `main.go`.
- [ ] Connect to local Postgres instance.

## Session 5: Testing & Verification
- [ ] Use `curl` to test successful/failed login.
- [ ] Project Wrap-up.