# moukrea/apt-repo

Debian/Ubuntu APT package repository, hosted on GitHub Pages.

## Adding the Repository

```bash
# Add GPG key
curl -fsSL https://moukrea.github.io/apt-repo/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/moukrea.gpg

# Add repository
echo "deb [signed-by=/usr/share/keyrings/moukrea.gpg] https://moukrea.github.io/apt-repo stable main" | \
  sudo tee /etc/apt/sources.list.d/moukrea.list

sudo apt update
```

## Available Packages

| Package | Description |
|---------|-------------|
| `opaq` | Credential manager — keeps secrets out of terminals, context windows, and command output |

Install any package with:

```bash
sudo apt install <package-name>
```
