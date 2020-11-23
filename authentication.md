# Libraries and Frameworks

Table of Contents
=================

   * [Session Vs Token](#Session-Vs-Token)



## Session Vs Token
Session is an Authentication Strategy where auth state is managed on the serever.  
Token is an Authentication Strategy where auth state is managed on the browser.


# Session 
  Auth state is managed on the server, here is a general step      
1. user submit form to be processed
2. server will store session and return browser session id
3. session ID stored on browser cookie storage(key value storage)
4. browser sends cookies with future requests

#### Cons

- can be vulnerable for CSRF(cross-site request forgery) attack
- since session is stored on the server makes it difficult to scale up. 



# Token 


Authentication is managed on the client side.            
1. user submit login form to be processed                
2. server creates a JWT(JSON web token)     
3. browser stores jwt in local storage      
4. jwt added on authorization header on future requests. On the following format, Authorization:Bearer<token>


  #### Cons
- can be difficult to invalidate 
- can be hijacked by an attacker
  


