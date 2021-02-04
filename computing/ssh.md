Key Pairs


```bash
    # Note: Keys will only work is ~/.ssh and ~/ have correct Permissions
    chmod go-w ~/
    chmod 700 ~/.ssh

    ssh-keygen -t rsa
    ssh-add -K ~/.ssh/id_rsa
    nano ~/.ssh/config
    Host *
        UseKeychain yes
        AddKeysToAgent yes
        IdentityFile ~/.ssh/id_rsa
    Host example_host
        HostName example.server.net
        Port 12422
        User special
    cat ~/.ssh/id_rsa.pub | pbcopy
    ssh-copy-id -i ~/.ssh/id_rsa.pub user@example.com
    # ~/.ssh/authorized_keys  # public keys of passwordless users

    # Port forwarding Socks Proxy - on local client
    ssh -D 8999 dreamhost

    # To port forward
    ssh -L 5672:10.73.146.211:5672 username@hostname
```
