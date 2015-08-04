## Tails: A Complete Guide 

### Persistence

Journalists rely on their notes, and so the idea of an operating system that saves nothing between sessions may sound sub-optimal.

For this reason, Tails has the optional feature of persistence -- saving files in an encrypted volume which are accessible across separate sessions. 

This is useful for files you're working on, and encryption keys you use with Tails. (It's generally inadvisable to move keys off a Tails machine -- you should keep them compartmentalized and away from your regular computer operating system.)

### Configuration

When you boot up Tails for the first time, you're asked if you want more options. 

To configure Persistence, click on Applications in the top left corner and navigate to "Configure persistent volume" under the Tails menu. 

Tails will warn you about the ways that using persistence could undermine your security. It's worth reading these warnings, which have to do with the persistent volume being encrypted but not hidden. It's always important to remember that installing additional software such as browser plugins can undermine you identity. 

The data on your persistent volume is encrypted with a passphrase that should be very secure. Check out the passphrase section of Encryption Works for more info on how to create a good passphrase. 

![Configuring a persistent drive on Tails.](http://i.imgur.com/oZzpzI4.png)

The setup wizard will then ask you which facets of persistence you want to configure. What you need will depend on your situation, but we recommend enabling Personal Data, GnuPG, SSH Client, Pidgin, Claws Mail, and Browser Bookmarks. These are the tools you'll need to have secure, encrypted email threads and IM conversations, as well as store documents that are works-in-progress. (These will be located in **Places > Persistent**.

After Tails has finished configuring your persistent drive, you'll need to restart for the changes to take effect. The next time you start Tails up, you'll see a second option during startup, asking if you want to access the persistent volume. 

![Accessing the persistent volume during Tails startup.](http://i.imgur.com/UdxgeaM.jpg)

It's important to remember that you can still use Tails without the persistent volume. If you're not working with your email or documents, it's a good idea not to enable persistence for regular browsing sessions to fully maintain your anonymity.

For more information, the Tails documentation has a [section](https://tails.boum.org/doc/first_steps/persistence/configure/index.en.html) on persistent volumes.