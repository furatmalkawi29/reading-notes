
# What's OAuth?

OAuth, which stands for “Open Authorization,” allows third-party services to exchange your information without you having to give away your password. 

It is an authorization framework for delegated access to APIs. It involves clients that request scopes that Resource Owners authorize/give consent to. Authorization grants are exchanged for access tokens

OAuth doesn't share password data but instead uses authorization tokens to prove an identity between consumers and service providers.
 OAuth is an authentication protocol that allows you to approve one application interacting with another 

<br>

## Roles

1. The Third-Party Application: "Client"

2. The API: "Resource Server"

3. The Authorization Server

4. The User: "Resource Owner"

![](https://a.slack-edge.com/fbd3c/img/api/articles/oauth_scopes_tutorial/slack_oauth_flow_diagram.png)

## Authorization
 
first step of OAuth2 is to get authorization from the user. 
For browser-based or mobile apps, this is usually accomplished by displaying an interface provided by the service to the user.


## grant types

1. Authorization Code  : for apps running on a web server, browser-based and mobile apps
2. Password:  for logging in with a username and password (only for first-party apps)
3. Client credentials: for application access without a user present
Implicit: was previously recommended for clients without a secret, but has been superseded by using the Authorization Code grant with PKCE.


<br> 

# Single-Page Apps

Single-page apps (or browser-based apps) run entirely in the browser after loading the source code from a web page.
 Since the entire source code is available to the browser, they cannot maintain the confidentiality of a client secret,
 so the secret is not used in this case .



