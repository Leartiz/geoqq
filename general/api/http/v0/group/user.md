# User 👨‍💻

## GET /api/my-profile

### Parameters
#### Required
- accessToken=`"<jwt-string>"`

### Responses
- *200*
```json
{
    "username": "<string>",
    "about-me": "<string>",
    "avatar": "<base58-string>",
    "privacy": {
        "hit-me-up": "<int>"
    }
}
```
- Other error codes.

## PUT /api/my-profile

### Request body
```json
{
    /* required */
    "access-token": "<jwt-string>",
       
    /* optional */
    "about-me": "<string>",
    "avatar": "<base58-string>",
    "privacy": {
        "hit-me-up": "<int>"
    }
}
```

### Responses
- *200*
- Other error codes.

<!-- -------------------------------------------- -->

## GET /api/users/{`userId`}

### Parameters
#### Required
- accessToken=`"<jwt-string>"`

### Responses
- *200*
```json
{
    "username": "<string>",
    "description": "<string>",
    "avatar": "<base58-string>",
    "is-mate": "<bool>"
}
```
- Other error codes.