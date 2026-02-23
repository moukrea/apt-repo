# moukrea/apt-repo

APT package repository for opaq, hosted on GitHub Pages.

## Installation

```bash
# Add GPG key
curl -fsSL https://moukrea.github.io/apt-repo/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/moukrea.gpg

# Add repository
echo "deb [signed-by=/usr/share/keyrings/moukrea.gpg] https://moukrea.github.io/apt-repo stable main" | \
  sudo tee /etc/apt/sources.list.d/moukrea.list

# Install
sudo apt update && sudo apt install opaq
```

## Upgrade

```bash
sudo apt update && sudo apt upgrade opaq
```

## Uninstall

```bash
sudo apt remove opaq
```
