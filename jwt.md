# Json Web Tokens

A json web token is just a secure way to send information back and forth. It is authenticating a user to be able to do something with whatever thing that you built. The structure goes as follows there is a Header, Payload , and signature and a jwt goes as follows xxxxx.yyyyy.zzzzz.

To break it down even further a header has two parts. The type of token which is our JWT and the signing algorithm. The payload contains the claims which are statements about an entity or an additional user. The signature you have to take everything listed above and sign that.