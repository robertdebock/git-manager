# Initial setup
Save these variables in a vault:
- vault_github_username
- vault_github_token

Run `ansible-vault create vault.yml`.

# Preparation

```
vagrant up
```

# Create releases

Automatically create releases of all repositories.

```
ansible-playbook create-release.yml --ask-vault-pass
```
