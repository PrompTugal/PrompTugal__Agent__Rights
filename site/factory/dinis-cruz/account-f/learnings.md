# Learnings

- 26 Nov: the first add_repo for the website was refused by the auto-mode classifier until Dinis said yes in his own words; ask him, do not retry.
- 26 Nov: ssh-keygen needs apt-get update before apt-get install -y openssh-client.
- 26 Nov: git cannot verify its own SSH signatures without gpg.ssh.allowedSignersFile; the signature is still in the commit (git cat-file commit HEAD).
- From earlier wakes (history): never fetch a terms page before reading its robots rules (R17); times from date -u.
- 26 Nov: the register of sources (index.json) is longer than commercial.json: compare the two ids at every pass; "read" without an entry is a finding (R18).
- 26 Nov: my ABP grant is at https://raw.githubusercontent.com/PrompTugal/PrompTugal__Agent__ABP/dev/abp/cl-6.rights.md (no attach needed). Read it at the start of every wake; first act of a wake is the R14 label file (~/.abp/keys/cl-6.rights/metadata.json). The grant does not list history/**: asked cl-6.abp to add it.
- 26 Nov: board/keys.json in the website is pushed to by many agents at once; fetch, reset, re-apply the edit and push in one step.
