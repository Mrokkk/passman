# passman
Simple password manager

## Usage
```
usage: passman [-h] {set,get} ...

positional arguments:
  {set,get}   sub-command help

optional arguments:
  -h, --help  show this help message and exit
```
Application keeps all passwords in the passkey encrypted file. Everytime you want to get or set the password you'll be asked for a passkey. Passkey is set on the first run of the `passman` when database file is created.
### Set
```
usage: passman set [-h] [-s SIZE] domain

positional arguments:
  domain

optional arguments:
  -h, --help            show this help message and exit
  -s SIZE, --size SIZE  Length
```
The above command creates a new entry in the database file for a `domain` with a random password with a lenght of `length` characters. Generated password would be copied into the clipboard.

### Get
```
usage: passman get [-h] domain

positional arguments:
  domain

optional arguments:
  -h, --help  show this help message and exit

```
The above command reads a password for a `domain` entry and pastes it to the clipboard.
