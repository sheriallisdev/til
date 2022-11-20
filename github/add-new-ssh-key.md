# Add a new SSH key to GitHub

## Generate a new SSH key

```shell
ssh-keygen -t ed25519 -C "your_email@example.com"
```

## Add SSH key to ssh-agent

```shell
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

## Add the new SSH key to your GitHub account

- Copy the contents of the `~/.ssh/id_ed25519.pub` file.

```shell
clip < ~/.ssh/id_ed25519.pub
```

- Go to the [SSH and GPG keys page on GitHub.com](https://github.com/settings/keys)
- Click on the New SSH key button and paste the contents of the SSH key
