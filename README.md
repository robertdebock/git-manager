# Initial setup
Save these variables in a vault:
- vault_github_username
- vault_github_token

Run `ansible-vault create vault.yml`.

# Preparation

```
ansible-galaxy install -r requirements.yml
vagrant up
```

# Create releases

Automatically create releases of all repositories.
```
./create-release.yml --ask-vault-pass
```

Create release for selected levels:
```
./create-release.yml --ask-vault-pass --tags level0
```
