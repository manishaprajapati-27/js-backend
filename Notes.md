# HTTP

Difference between HTTP and HTTPs
HTTP : Sends the clear data that is readable from server to client.
HTTPs : Sends the data in Encrypted form that is readable when data show in server.

How to Transfer Text?

App -><- Server

Communication between server and client is done by http.

URL, URI, URN

## What are HTTP Headers

1. Metadata -> Key value sent along with request and response
2. Caching , Authentication, Manage state
   x-Prefix used in before 2012(X-deprecated)
3. Request Header -> From Client
4. Response Header -> From Server
5. Representation Headers -> Encoding/Compression
6. Payload Headers -> Data(Send Data)

## Most Common Headers

1. Accept : Application/Json
2. User - Agent
3. Authentication
4. Content - Types(Images, Files, etc)
5. Cookie
6. Cache - Control

## CROS

1. Access - Control - Allow - Origin
2. Access - Control - Allow - Credential
3. Access - Control - Allow - Method

## Security

1. CROS - Origin - Embedder - Policy
2. CROS - Origin - Opener - Policy
3. Content- Security - Policy
4. X - XSS - Protection

## HTTP Methods

Basic set of operations that can be used to interact with server

1. GET : Retrieve a resource
2. HEAD : No message body (response headers only)
3. OPTIONS : What operations are available
4. TRACE : Loopback test (get same data)
5. DELETE : Remove a resourse
6. PUT : Replace a resourse
7. POST : Interact with resource(mostly add)
8. PATCH : Change part of a resource

## HTTP Status code

1xx - Informational
2xx - Success
3xx - Redirection
4xx - Client Error
5xx - Server Error

100 - Continue
102 - Processing
200 - Ok
201 - Created
202 - Accepted
307 - Temporary redirect
308 - Permanent redirect
400 - Bad request
401 - Unauthorized
402 - Payment request
404 - Not Found
500 - Internal Server Error
504 - Gateway time out



## Middle Ware 

Before send the request we "check" somethings. The Check is called Middleare (Jaate hue mujhse mil ke jaana).

## Use of Postman 
1. Make new Collection
2. Make new Environment
3. Give name to environment then use it
4. {{}} use variable in double curly brac
5. Save 

## About Database Information
1. Database always present in onather Continents
2. If you know data is take time to came then use await always.
3. Remember always await in async await else it throw error

## About Access token and Refresh token

Access token is generate and it's expired fast.
Refresh token is saved on Database and it's expired late as compare to access token.
After login the user in cookies generate two token access and refresh respectivelly.
If user send request then it match new access token to refresh token and give new refresh and access token.

## Aggregation in MongoDB

[
    {

$lookup: {
    from:
    localField:
    foreiginField:
    as:
}
    },
    {
        $addFields:{
            author_details: {
                $arrayElement : ["$author_details", 0]
            }
        }
    }
]

In aggregate To add pipelines inside of pipeline we can add nested pipeline using "pipeline" keyword
In aggregate pipelines mongoose is not work.









