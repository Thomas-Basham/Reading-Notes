# Class 34

## Reading

### [Django Settings Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)
- There is no built-in universal way to configure Django settings without hardcoding them.
- Hide SECRET_KEY in .env
- os.environ can be tricky sometimes and require additional effort to handle errors
- Its "better" to use django-environ 
- Django Settings: Best practices

        Keep settings in environment variables.
        Write default values for production configuration (excluding secret keys and tokens).
        Don’t hardcode sensitive settings, and don’t put them in VCS.
        Split settings into groups: Django, third-party, project.
        Follow naming conventions for custom (project) settings.


### [SSH Tutorial](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)

What Is SSH?

- SSH, or Secure Shell Protocol, is a remote administration protocol that allows users to access, control, and modify their remote servers over the internet
- SSH service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner
- The most popular SSH client is PuTTY
- The SSH command consists of 3 distinct parts:

        ssh {user}@{host}
- The SSH key command instructs your system that you want to open an encrypted Secure Shell Connection
- {user} represents the account you want to access
- {host} refers to the computer you want to access
- This can be an IP Address (e.g. 244.235.23.19) or a domain name (e.g. www.xyzdomain.com)
- There are three different encryption technologies used by SSH:

        
        Symmetrical encryption
        Asymmetrical encryption
        Hashing
- Symmetric encryption is a form of encryption where a secret key is used for both encryption and decryption of a message by both the client and the host
- Unlike symmetrical encryption, asymmetrical encryption uses two separate keys for encryption and decryption 
- These two keys are known as the public key and the private key 
- Together, both these keys form a public-private key pair
- One-way hashing is another form of cryptography used in Secure Shell Connections 
- One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted 
- They generate a unique value of a fixed length for each input that shows no clear trend which can be exploited
- The way SSH works is by making use of a client-server model to allow for authentication of two remote systems and encryption of the data that passes between them
- The final stage before the user is granted access to the server is authenticating his/her credentials. For this, most SSH users use a password
- The user is asked to enter the username, followed by the password
- These credentials securely pass through the symmetrically encrypted tunnel, so there is no chance of them being captured by a third party

## Bookmark and Review

### [White Noise](http://whitenoise.evans.io/en/stable/)

### [IaaS](https://en.wikipedia.org/wiki/Infrastructure_as_a_service)

### [PaaS](https://en.wikipedia.org/wiki/Platform_as_a_service)

### [CORS](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)