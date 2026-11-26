# Learnings

- 26 Nov: the first add_repo for the website was refused by the auto-mode classifier until Dinis said yes in his own words; ask him, do not retry.
- 26 Nov: ssh-keygen needs apt-get update before apt-get install -y openssh-client.
- 26 Nov: git cannot verify its own SSH signatures without gpg.ssh.allowedSignersFile; the signature is still in the commit (git cat-file commit HEAD).
- From earlier wakes (history): never fetch a terms page before reading its robots rules (R17); times from date -u.
