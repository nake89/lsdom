# lsdom
CLI tool to list domains (for certain user by username or domain or for all users) in cpanel.

### Usage
```
Usage: lsdom [OPTION] [INPUT]
Example: lsdom [cPanel username]
Lists domains for certain user by username or domain or for all users

Options:
  -d [domain]      Displays all domains  of the user of the input domain.
  -a, --all        Lists all domains.
  -v, --version    Displays version.
  -h, --help       This help page.
```

### Prerequisites
**jq** is needed for json parsing. cPanel api gives out the result in json, which is why it is needed. You can install it simply by typying the below in to the terminal:
```
yum install jq
```

### Installing
```
mkdir ~/bin
cd ~/bin
echo export PATH=\$PATH:$PWD >> ~/.bashrc
source ~/.bashrc
cd ~
git clone https://github.com/nake89/lsdom
mv lsdom/ .lsdom
cd .lsdom
chmod u+x lsdom
ln -s ~/.lsdom/lsdom ~/bin/lsdom

```
