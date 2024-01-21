# ENCRYPTION---CRYPTO-101
TRY HACKME ENCRYPTION - CRYPTO 101
ncryption- Crypto 101 WriteUp — TryHackMe

I tried to prepare a write-up for the “Encryption — Crypto 101” room on tryhackme.
(Task 1)- What will this room cover?
Why cryptography matters for security and CTFs
The two main classes of cryptography and their uses
RSA, and some of the uses of RSA
2 methods of Key Exchange
Notes about the future of encryption with the rise of Quantum Computing
#1 I’m ready to learn about encryption
ANSWER: No answer needed
(Task 2)- Key terms
Many of these key terms are shared with https://tryhackme.com/room/hashingcrypto101
#1 I agree not to complain too much about how theory heavy this room is.
ANSWER: No answer needed
#2 Are SSH keys protected with a passphrase or a password?
Passphrase: Separate to the key, a passphrase is similar to a password and used to protect a key.
ANSWER: passphrase
(Task 3)- Why is Encryption important?
Cryptography is used to protect confidentiality, ensure integrity, ensure authenticity. You use cryptography every day most likely, and you’re almost certainly reading this now over an encrypted connection.
#1 What does SSH stand for?
Secure Shell (SSH) is a cryptographic network protocol for operating network services securely over an unsecured network.
ANSWER: Secure Shell
#2 How do web servers prove their identity?
When you connect to your bank, there’s a certificate that uses cryptography to prove that it is actually your bank rather than a hacker.
ANSWER: certificates
#3 What is the main set of standards you need to comply with if you store or process payment card details?
Whenever sensitive user data needs to be stored, it should be encrypted. Standards like PCI-DSS state that the data should be encrypted both at rest (in storage) AND while being transmitted. If you’re handling payment card details, you need to comply with these PCI regulations.
ANSWER: PCI-DSS
(Task 4)- Crucial Crypto Maths
There’s a little bit of math(s) that comes up relatively often in cryptography. The Modulo operator. Pretty much every programming language implements this operator, or has it available through a library. When you need to work with large numbers, use a programming language. Python is good for this as integers are unlimited in size, and you can easily get an interpreter.
#1 What’s 30 % 5?
ANSWER: 0
#2 What’s 25 % 7
ANSWER: 4
#3 What’s 118613842 % 9091
just google it

ANSWER: 3565
(Task 5)- Types of Encryption
#1 Should you trust DES? Yea/Nay
ANSWER: Nay
#2 What was the result of the attempt to make DES more secure so that it could be used for longer?
The algorithm is believed to be practically secure in the form of Triple DES, although there are theoretical attacks.
ANSWER: Triple DES
#3 Is it ok to share your public key? Yea/Nay
ANSWER: Yea
(Task 6)- RSA — Rivest Shamir Adleman
#1 p= 4391, q= 6659. What is n?
ı use on this website.

ANSWER: 29239669
#2 I understand enough about RSA to move on, and I know where to look to learn more if I want to.
ANSWER: No answer needed
(Task 7)-Establishing Keys Using Asymmetric Cryptography
#1 I understand how keys can be established using Public Key (asymmetric) cryptography.
ANSWER: No answer needed
(Task 8)- Digital signatures and Certificates
Digital signatures are a way to prove the authenticity of files, to prove who created or modified them. Using asymmetric cryptography, you produce a signature with your private key and it can be verified using your public key. As only you should have access to your private key, this proves you signed the file. Digital signatures and physical signatures have the same value in the UK, legally.
#1 What company is TryHackMe’s certificate issued to?

ANSWER: CloudFlare
(Task 9)- SSH Authentication
#1 I recommend giving this a go yourself. Deploy a VM, like Learn Linux and try to add an SSH key and log in with the private key.
ANSWER: No answer needed
#2 Download the SSH Private Key attached to this room.
ANSWER: No answer needed
#3 What algorithm does the key use?

ANSWER: RSA
#4 Crack the password with John The Ripper and rockyou, what’s the passphrase for the key?
ı use this commands:
/usr/share/john/ssh2john.py [downloaded file location] > [new file name]
john [new file name] --worldlist=[rockyou.txt file location]
ANSWER: delicious
(Task 10)- Explaining Diffie Hellman Key Exchange
Key exchange allows 2 people/parties to establish a set of common cryptographic keys without an observer being able to get these keys. Generally, to establish common symmetric keys.
#1 I understand how Diffie Hellman Key Exchange works at a basic level
ANSWER: No answer needed
(Task 11)- PGP, GPG and AES
#1 Time to try some GPG. Download the archive attached and extract it somewhere sensible.
ANSWER: No answer needed
#2 You have the private key, and a file encrypted with the public key. Decrypt the file. What’s the secret word?
ı use this commands:
unzip gpg.zip

sudo gpg --import tryhackme.key

sudo gpg message.gpg

ls

cat message
ANSWER: Pineapple

