## Tails: A Complete Guide 

### Creating PGP Keys

GnuPG (also known as PGP or GPG) is free software you can use to encrypt your email messages and other files on your computer. Tails encrypts your files by default, but PGP encryption is useful if you want to email those files or store them somewhere else. 

This chapter assumes you know about public and private keys. For more information, check out the PGP section of Encryption Works. <link goes here> Before going much further, you should also have Persistence installed.

#### Setup 

On the Tails desktop, there's a clipboard icon in the top right corner. From there, you can access a drop-down menu and manage your keys. If you click on GnuPG keys, you'll see that Tails already has the public keys of the Tails team, so you can securely contact the developers with questions or bug reports.

From here, we're going to create a set of PGP keys to use with Tails. Generally speaking, it's not a good idea to shuttle keys between a Tails machine and an insecure operating system.)

Navigating to **File > New**, we're going to create a new PGP key.

After entering the key's name and email address, select key options. (Unless you have a compelling reason to, I recommend leaving the comment field blank.)

![Creating a PGP keypair.](http://i.imgur.com/kT5ssxi.png)

Selecting RSA encryption is a good choice. 2048 is generally the smallest key you can securely use, and we recommend bumping that up to 4096. 

Everyone has their own opinions on key expiry -- while some people maintain that keys don't need to or shouldn't expire, we recommend setting the expiry date to five years in the future. This allows you to use the key for an extended period of time but if you lose the key, it will eventually fall out of us. 

You'll then be asked for a passphrase. Again, this should be long and secure. For information about creating a strong passphrase, check out Encryption Works. 

Then, the key will generate and you'll see the new key pair in the GnuPG list. If you've configured persistence, the keys will be saved. If not, the private and public key will be wiped when you shut down. For information on configuring Persistence, click here.

### Encrypting And Decrypting

Once you've created a PGP keypair, encrypting a file just involves right-clicking the file and selecting _Encrypt_.

![Encrypting a file on Tails.](http://i.imgur.com/j04K822.png) 

From here, you'll select the key you want to encrypt the file to. If you encrypt it to your own public key, this adds another layer of security to Tails and also allows you to back up the file on another storage device. 

This creates a second file, named the same as the original but ending in _.pgp_. This is the encrypted file.

![Two files on the desktop.](http://i.imgur.com/5eNGinS.png)

Double-clicking the file prompts you to enter your PGP passphrase In this example, I encrypted the file to myself. Had I encrypted it with someone else's public key, they would need their private key to decrypt it. 

![Decryption.](http://i.imgur.com/0YYYIzM.png)