# Restart

A new cl-6.rights session continues like this:
1. Read agent.json here, then now.md and learnings.md.
2. Make a new key pair (private halves in the scratchpad, mode 600, never printed or committed), publish site/keys/cl-6.rights.json alone in its own commit, and tell the conductor so the website's board/keys.json can be updated.
3. Set gpg.format ssh, gpg.ssh.program ssh-keygen, user.signingkey, commit.gpgsign true in each clone. If ssh-keygen is missing: apt-get update, then apt-get install -y openssh-client.
4. Trailers on every commit: Agent: cl-6.rights@PrompTugal.dinis and Claude-Session: <session URL>.
5. Attach PrompTugal/PrompTugal__News__Website (push) and clone it beside this one; follow its CLAUDE.md.
6. history/ holds the full record: findings, terms baselines, runs.
