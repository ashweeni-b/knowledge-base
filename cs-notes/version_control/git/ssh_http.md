### SSH vs HTTPS

SSH and HTTPS both are methods to connect the local machine to a remote repo
<br />

_SSH (Secure Shell)_

- A protocol used for secure remote access and authentication
- Used in Git via SSH keys

| SSH Pros | SSH Cons |
| -------- | ------- |
| Better security compared to HTTPS | Setting up and managing SSH keys may be more complex |
| Uses public-key cryptography which enhances authentication security | Communication may be restricted by firewall |
| Streamlines authentication process |  |

<br />

_HTTPS (Hyper Text Transfer Protocol Secure)_
- A protocol used for secure communication over the web
- Used in browsers and Git via tokens


| HTTPS Pros | HTTPS Cons |
| -------- | ------- |
| More straightforward setup compared to SSH | SSH is considered more secure |
| Authenticate with an username and password or with a personal access token if using GitHub | User may need to enter their credentials frequently. Credential caching tools may be used to avoid this issue. For example, Credential Manager in Windows  and Keychain Access in Mac |
| More compatible with firewalls |  |

---