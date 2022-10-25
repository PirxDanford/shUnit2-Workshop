# Installation

## Linux/Unix

### Apt
```console
apt-get update
apt-get install shunit2
```

### Apk
```console
apk add shunit2
```

When using it in a Dockerfile it is good practice to include the `--no-cache` flag.
```console
apk add --no-cache shunit2
```

### From sourcecode
```console
curl -sLo /usr/local/bin/shunit2 https://raw.githubusercontent.com/kward/shunit2/master/shunit2
chmod +x /usr/local/bin/shunit2
```

## Mac OS X
```console
brew install shunit2
```

## Windows
Via bash and apt as above (untested): 
https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/

or via Cygwin, included in https://mobaxterm.mobatek.net/

from within MobaXterm start a local shell and install from source

```console
curl -sLo /usr/bin/shunit2 https://raw.githubusercontent.com/kward/shunit2/master/shunit2
chmod +x /usr/bin/shunit2
```

# Troubleshooting

In case of installation issues, please provide feedback via the issues section, or share your remediation with a PR.
