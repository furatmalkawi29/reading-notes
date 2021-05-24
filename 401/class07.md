
## Write the following steps in the correct order:

- Register your application to get a client_id and client_secret
- Ask the client if they want to sign in via a third party
- Redirect to a third party authentication endpoint
- Receive authorization code
- Make a request to a third-party API endpoint
- Receive access token
- Make a request to the access token endpoint



## TERMS 

1. client ID : 
public identifier for "public" apps  that supports OAuth 
example : 

- Instagram: f2a1ed52710d4533bde25be6da03b6e3

- SoundCloud: 269d98e4922fb3895e9ae2108cbb5064

2. client secret : used for "private" apps , only known by application and the authorization server . 


3. Authentication Endpoint : mechanism used to verify the identity of a network's  connecting device .

4. token endpoint : is where apps make a request to get an access token for a user  

5. API endpoint : is the point of  communication when two systems are interacting. It refers to  communication between an API and a server.

6. authorization code:  is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server


7. Access tokens: used in token-based authentication to allow an application to access an API . 

<br> 
<hr>

- What can you do with an authorization code?

 see what the information the client is requesting, and approve or deny the request, exchange for an access token

- What can you do with an access token?

 use to make API requests

- What’s a benefit of using OAuth instead of your own basic authentication?

 With Basic authentication the full credentials are always included in each request, while with OAuth it's the access token that is included in each request.


<br> 
<hr>

   
<br><br>

# JSON WEB TOKENS 

Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

The output is three Base64-URL strings separated by dots that can be easily passed in HTML and HTTP environments

## How do JSON Web Tokens work?

In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. 

![](https://cdn.auth0.com/blog/legacy-app-auth/legacy-app-auth-5.png)