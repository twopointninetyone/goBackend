# go backend
- very nice

# Planned Structure (probably):

## Request Structure:
```go
type request struct {
    User string `json:"user"`
    Password string `json:"pass"`
    SessionKey string `json:"sessionKey"`
}
```
Password is required for login/registration \n
SessionKey is required for other user actions \n
(Only one of them is needed) \n
