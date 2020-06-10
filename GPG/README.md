
![gnuPG ontop of openPGP pretty good privacy](https://i.imgur.com/Vma72N0.png)

What can you do with GPG?

you can add a signature to your github commits.

receive or send encrypted message + signature.

encrypt your files, or add signature to files.

add your signature to others master public key.

post message online with your signature.



```
--- MASTER PRIV KEY ----------------- 

ability: [certify] - create subkeys 
                                      
--- MASTER PUB KEY ------------------ 
                                      
includes: UID (name, email, comment),  
          subkeys fingerprint,       
          expire dates, signatures     
                                      
------------------------------------- 





--- SUB PRIV KEY --------------------

ability: [encrypt] - files or text

--- SUB PRIV KEY --------------------

ability: [sign] - add signature to
         messages, files, or add your
         signature to other users
         master public key

--- SUB PRIV KEY --------------------

...

```

generate master keypair with options `--expert` and `--full-gen`, then
afterwards you can `--edit-key` to add subkeys. to have the same setup
as above.

