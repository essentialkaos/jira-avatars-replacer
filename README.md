<p align="center"><a href="#readme"><img src="https://gh.kaos.st/jira-avatar-replacer.svg"/></a></p>

<p align="center">
  <a href="https://github.com/essentialkaos/jira-avatars-replacer/actions"><img src="https://github.com/essentialkaos/jira-avatars-replacer/workflows/CI/badge.svg" alt="GitHub Actions Status" /></a>
  <a href="#license"><img src="https://gh.kaos.st/apache2.svg"></a>
</p>

<p align="center"><a href="#installation">Installation</a> • <a href="#usage">Usage</a> • <a href="#license">License</a></p>

<br/>

`jira-avatar-replacer` is a simple tool for updating JIRA avatars to HQ versions.

### Installation

#### From GitHub repository

```bash
# Download rsz utility for images resizing
bash <(curl -fsSL https://apps.kaos.st/get) rsz
# Download utility
curl -fL# -o jr https://kaos.sh/jira-avatars-replacer/jr
chmod +x jr
sudo mv jr rsz /usr/bin/
```

Also, you can use the latest version of utility without installation (_but you have to install_ [`rsz`](https://kaos.sh/rsz) _utility first_):

```bash
bash <(curl -fsSL https://kaos.sh/jira-avatars-replacer/jr) # pass options here
```

### Usage

```
Usage: jr {options} image avatar-id

Options

  --super, -s        Super resolution (x4)
  --no-color, -nc    Disable colors in output
  --help, -h         Show this help message
  --version, -v      Show information about version

Examples

  JIRA_DIR=/opt/jira-data sudo jr image.png 18311
  Update avatar with ID 18311

```

### License

[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0)

<p align="center"><a href="https://essentialkaos.com"><img src="https://gh.kaos.st/ekgh.svg"/></a></p>
