# RecRanger's Pywallet Fork

A fork of [jackjack-jj's pywallet](https://github.com/jackjack-jj/pywallet), better maintained
and ready for Python 3 usage on modern systems.

## Status

This fork aims to incrementally refactor Pywallet into a more maintainable configuration. 

### Working Features

* None yet

### Upcoming Features

* Data recovery tool

### Unsupported Features

* Everything else :(


## Usage

```
Usage: pywallet.py [options]

Options:
  --version             show program's version number and exit
  -h, --help            show this help message and exit
  --dumpwallet          dump wallet in json format
  --importprivkey=KEY   import private key from vanitygen
  --importhex           KEY is in hexadecimal format
  --datadir=DATADIR     wallet directory (defaults to bitcoin default)
  --wallet=WALLETFILE   wallet filename (defaults to wallet.dat)
  --label=LABEL         label shown in the adress book (defaults to '')
  --testnet             use testnet subdirectory and address type
  --namecoin            use namecoin address type
  --otherversion=OTHERVERSION
                        use other network address type, whose version is
                        OTHERVERSION
  --info                display pubkey, privkey (both depending on the
                        network) and hexkey
  --reserve             import as a reserve key, i.e. it won't show in the
                        adress book
  --balance=KEY_BALANCE
                        prints balance of KEY_BALANCE
  --web                 run pywallet web interface
  --port=PORT           port of web interface (defaults to 8989)
```

## Dependencies

### Debian-based Linux
```bash
sudo apt install build-essential python3 python3-dev python-bsddb3
```

### Mac OS X:
 1. Install MacPorts from http://www.macports.org/
 2. Install:
 
```bash
sudo port install python27 py27-pip py-bsddb python_select
sudo easy_install ecdsa
```
