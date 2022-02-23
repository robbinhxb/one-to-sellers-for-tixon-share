# one-to-sellers-for-tixon-share
tixon share
Setup
$ sudo gem install ejson ejson2env
then obtain the necessary keypair and place it in /opt/ejson/keys/.

Usage
Run the following command to decrypt the secrets into the environment:

eval $(ejson2env secrets.ejson)
Managing secrets.ejson
To decrypt secrets.ejson for modification, run:

$ ejson decrypt secrets.ejson -o secrets_unencrypted.ejson
Edit, then run the following to re-encrypt the file BEFORE COMMITING YOUR CHANGES:

$ ejson encrypt secrets_unencrypted.ejson
$ mv secrets_unencrypted.ejson secrets.ejson

Setup$ sudo gem install ejson ejson2env

then obtain the necessary keypair and place it in /opt/ejson/keys/.

UsageRun the following command to decrypt the secrets into the environment:

eval $(ejson2env secrets.ejson)

Managing secrets.ejsonTo decrypt secrets.ejson for modification, run:

$ ejson decrypt secrets.ejson -o secrets_unencrypted.ejson

Edit, then run the following to re-encrypt the file BEFORE COMMITING YOUR CHANGES:

$ ejson encrypt secrets_unencrypted.ejson
$ mv secrets_unencrypted.ejson secrets.ejson
