# go backend
- very nice

# Planned Structure (probably):

## Request Structure:
```go
type request struct {
    User string `json:"user"`
    Password string `json:"pass,omitempty"`
    SessionKey string `json:"sessionKey,omitempty"`
}
```
Password is required for login/registration  
SessionKey is required for other user actions  
(Only one of them is needed)

## Response Structure:
```go
type response struct {
    SessionKey string `json:"sessionKey,omitempty"`
    Result map[string]any `json:"result,omitempty"`
}
```
SessionKey is added if the user logs in  
Result is added if the command gives any  
yeah  
