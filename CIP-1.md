Title
-----

U°Community active key login

U°OS Improvement Proposal
-------------------------

Add active key registration and authorization.

Users should be able to log in via active key and save key pairs during registration. Brainkey can be used for recovery.
During the registration process, a password-encrypted json file with account private keys can be saved, and a brainkey is displayed for user to write it down and use later for account keys recovery.
During the login process a plain text key or an encrypted json can be used for authorization.
Impact
-------

Users will be able to use active private key to log in. Accounts, created via cleos or any other way that includes owner and active keys, will be accessible via the U°Community interface. Right now you can not log into your account on U°Community if you've registered your account via active and owner authorities. There is now way to reverse-generate a brainkey for those pairs.

Active key doesn't compromise the owner authority of an account, like the brainkey does. Without active key login accounts, registered with key pairs, won't be accessible via the U°Community interface. At the same time, you can't get access to the keys for accounts registered via U°Community.
