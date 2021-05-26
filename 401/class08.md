
## When is Basic Authorization used vs. Bearer Authorization?

Basic Auth
 
The basis Auth allow you to access the API directly with your credential : user/password.

This authentication method is useful when you need to check identity and get the data in one call. 

<br>

Bearer Token


To access the API with a bearer token you will need to make 2 call :

one to get the bearer token (from basic auth) and one to get the data


## What does the JSON Web Token package do?

standard used to create access tokens for an application. 

the server generates a token that certifies the user identity, and sends it to the client.

The client will send the token back to the server for so the server knows the request comes from a particular user.

## What considerations should we make when creating and storing a SECRET?

 Add it in as an enviromental variable and use .gitignore

 not share it on messeging apps


 <br>

## Document the following Vocabulary Terms

encryption

is the process that rearranges readable text so it can only be read by the person who has the secret code. It helps provide data security for sensitive information.

token 

tiny piece of code that contains a large amount of data about the user, permissions . used when you use credentials from one website (like Facebook) to gain entry to another website (like soundcloud) 

bearer

Bearer authentication involves security tokens called bearer tokens. The name “Bearer authentication” can be understood as “give access to the bearer of this token.” .

secret 

The secret value, contained within a token, which is used to derive token 


JSON Web Token

standard used to create access tokens for an application. 


<br>

# RBAC 

RBAC is the idea of assigning system access to users based on their role in an organization.

## Benefits of RBAC?

With the proper implementation of RBAC, the assignment of access rights becomes systematic and repeatable. Further, it is much easier to audit user rights, and to correct any issues identified.

RBAC may sound intimidating, but it can in reality be easy to implement, and will make the ongoing management of access rights much easier and more secure.