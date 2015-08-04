## Tails: A Complete Guide 

### Introduction To Tails

> "[Tails] has been an essential tool for reporting the NSA story. It is an all-in-one secure digital communication system (GPG email, OTR chat, Tor web browser, encrypted storage) that is small enough to swallow."
> — Laura Poitras, Oscar-winning documentary filmmaker and board member with Freedom of the Press Foundation.

Software is said to be either "open-source" or "closed-source," depending on whether security researchers and independent auditors can look at the code, see what it does, and make sure that nothing untoward is happening. 

Mac OS X and Windows are examples of closed-source operating systems. Tim Cook, Apple's CEO, has [claimed](https://www.apple.com/privacy/) that the U.S. government doesn't have backdoor access to Apple products, but since we can't look at the code ourselves, we're forced to take his word for it. Linux systems such as [Ubuntu](http://www.ubuntu.com) or [Debian](https://www.debian.org/) are open-source alternatives to Mac and Windows.

In 2009, the Tails operating system (OS) was released. Essentially, it's a version of Linux that's been modified to enhance user privacy and anonymity. It's currently the gold standard for secure, anonymous computer use, and was crucial to Ed Snowden when he worked with Freedom of the Press board-members Glenn Greenwald and Laura Poitras to reveal NSA overreach.

Every part of Tails is designed to strengthen the user's security. For instance, the system wipes itself clean every time you power down so that if your system is compromised by malware during one browsing session, it's gone the next time you boot up. 

![The Tails operating system.](https://raw.githubusercontent.com/tommycollison/encryption-works/issue_37_tails/images/tails_desktop.png)

### Main Features Of Tails

#### Runs Off External Storage Device

Tails is more secure than other operating systems in part because it runs on an external storage device -- a USB stick or a DVD. Most computers store the OS on an internal hard-drive, which makes them easier for malware and other malicious code to compromise them. Tails never touches your computer's hard-drive or BIOS, and remains entirely self-contained on the external storage device.

#### Wipes Upon Shutdown

Tails securely wipes everything you’ve done every time you shut it down. This means that you boot into a clean state every time you start Tails. This is for security reasons -- if you're the victim of malware or the target of a keylogger, there's no place for the virus for the virus to persist.

This means that if you want to work on documents or save GPG keys, you should enable another feature of Tails, called **Persistence**, whereby Tails saves certain files in an encrypted volume which is accessible across separate sessions. 

#### State-of-the-Art Cryptographic Tools Come Pre-Installed

Out of the box, Tails allows for easy use of GPG, OTR, and Tor software. Other secure tools, such as [HTTPS Everywhere](https://www.eff.org/https-everywhere) and [LUKS](https://en.wikipedia.org/wiki/LUKS) disk-encryption, also come as standard.

#### All Connections Go Through Tor

The Tor anonymity network comprises over 6,000 volunteer nodes which bounces your Internet traffic through intermediaries to anonymize it. One of the most popular ways of using Tor is with the web browser bundle, but this doesn't include other traffic, such as desktop-based mail and instant message chats. Tails routes all network connections through the Tor network so you can browse anonymously and circumvent censorship. 

