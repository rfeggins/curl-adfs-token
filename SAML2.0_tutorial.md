# SAML

SAML is a single sign on protocol used to authenticate access to an applications. While there are different SAML versions
the new industry standard is SAML2.0.

Also while there are other protocols, such as OAUTH2 that could be used, covering whether SAML or OAUTH is an appropriate solution 
for different scenarios is out of the scope of this post. 

# SAML Terms
There are a number of terms that need to be understood in order to get a firm grasp of SAML and SSO systems. The following terms are used by SAML specification and are needed to talk about deploying SSO solutions.

## Identity Provider (IDP) : 
The server the user will ultimately authenticate with. It can be thought of as an authorization authority that holds the user’s credentials. As an example, when logging into an application with your Facebook credentials, Facebook is considered the IDP.

## Service Provider (SP): 
The service or application that the user is trying to access. Slack or Github for example. This application doesn’t hold the job of authenticating the user but instead delegates it to the IDP.

## Client: 
The user that is sending a request to the SP.

## SSO or Single Sign on Service: 
Ths SSO service allows the user to access a single account and is often integrated with an IDP service

#The Logic behind SAML
The concepts behind a SAML flow are more easily understood than its implementation. There are two main user flows to grasp (both assume that the SP has existing knowledge of the IDP):

1. A user is trying to login to a service provider but the identity provider maintains knowledge of the user’s account. The user has not been authenticated yet and first needs to authenticate with an identity provider in order to gain access to the service provider.
2. A user has already authenticated with an identity provider and when trying to access a service provider, the user is granted access to the service provider immediately without having to authenticate with the IDP again.




https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/overview/ad-fs-scenarios-for-developers
