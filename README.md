# CAD Preprocess APT Repository

This repository hosts the APT packages for [CAD Preprocess](https://github.com/Harshil-Anuwadia/cad-preprocess).

## Installation

### Add Repository (Signed)

```bash
# Add GPG key
curl -fsSL https://harshil-anuwadia.github.io/cad-preprocess-apt/cad-preprocess.gpg \
  | sudo gpg --dearmor -o /usr/share/keyrings/cad-preprocess.gpg

# Add repository
echo "deb [signed-by=/usr/share/keyrings/cad-preprocess.gpg] \
  https://harshil-anuwadia.github.io/cad-preprocess-apt stable main" \
  | sudo tee /etc/apt/sources.list.d/cad-preprocess.list

# Install
sudo apt update
sudo apt install cad-preprocess
```

### Add Repository (Unsigned - Development Only)

```bash
echo "deb [trusted=yes] https://harshil-anuwadia.github.io/cad-preprocess-apt stable main" \
  | sudo tee /etc/apt/sources.list.d/cad-preprocess.list

sudo apt update
sudo apt install cad-preprocess
```

## Direct Download

Download the `.deb` file from the [pool](./pool/main/c/cad-preprocess/) directory.

## Links

- [Main Project Repository](https://github.com/Harshil-Anuwadia/cad-preprocess)
- [Documentation](https://harshil-anuwadia.github.io/cad-preprocess/)
- [Releases](https://github.com/Harshil-Anuwadia/cad-preprocess/releases)
