# go backend
- very nice

# Planned Structure (probably):

## Request Structure:
```go
type request struct {
    User string `json:"user"`
    Password string `json:"pass"`
    SessionKey string `json:"sessionKey"`
    /// either Password or SessionKey must be filled, password for login/registration, or session keys for other user actions
}
```
