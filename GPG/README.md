
![gnuPG ontop of openPGP pretty good privacy](https://i.imgur.com/Vma72N0.png)

```
--- MASTER PRIV KEY ----------------- 

ability: [certify] - create subkeys 
                                      
--- MASTER PUB KEY ------------------ 
                                      
+encoded: UID (name, email, comment),  
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
afterwards you can `--edit-key` to add subkeys.
