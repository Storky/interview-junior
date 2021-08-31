# HTTP APIs


## 1. WTF is Rest
Rest is architectural style to build HTTP API between services. Its using HTTP methods, client and server are stateless and can be changed independently.

## 2. What is gRPC
## 3. What is graphQL
## 4. Thrifts
## 5. HTTP methods

Main are GET,POST,PUT DELETE, HEAD, PATCH, OPTIONS
#### 1. which is save and idempotent
Save are: GET, OPTIONS, HEAD
Not save are: POST, PUT, DELETE 
Idempotent: PUT, GET, OPTIONS, DELETE, HEAD
Not idempotent: POST, PATCH
#### 2. status codes meaning
- Informational responses **100**
- Successful responses **200**
- Redirects **300**
- Client errors **400**
- Server errors **500**


## 6. Cookies

- Cookies is data, saved in small text files op PC, which is transfered by Head in Cookie field, additional param is valid time.

- How to delete - set valid time to past.
- isSecure and httpOnly params - isSecure checks for https, httpOnly makes invisible in JS.






