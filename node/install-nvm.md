# Install NVM

[nvm-sh/nvm repo](https://github.com/nvm-sh/nvm)

## Installation

```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

Check if the following has been added to your profile config file (~/.zshrc or ~/.bashrc), if not add it at the end of the file.

```shell
export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
```

## Verify Installation

```shell
command -v nvm
```

The above command should output `nvm` if installed correctly

## Usage

```shell
nvm install --lts #lts version
```

```shell
nvm install node # "node" is an alias for the latest version
```

```shell
nvm install 14.7.0 # or 16.3.0, 12.22.1, etc

```
