# Converting .ppk to .pem files on macOS and .pem to .ppk

## Steps For macOS .ppk to .pem

### Step 1

-----------

1 :- Open Terminal then install 

Press Command + Space Bar on your Mac keyboard (alternatively, press F4) Type in “Terminal”

```
brew install putty
```
OR


```
sudo port install putty
```

### Step 2

-----------

1:- in terminal type puttygen
```
puttygen
```

output look like same 

```
imranchaush@Imrans-MacBook-Air key % puttygen
Usage: puttygen ( keyfile | -t type [ -b bits ] )
                [ -C comment ] [ -P ] [ -q ]
                [ -o output-keyfile ] [ -O type | -l | -L | -p ]
Use "puttygen --help" for more detail.
```


### Step 3

-----------

1:- we will convert .pem to .ppk

```
puttygen key.ppk -O private-openssh -o key.pem
```
-O capital 

-o small

Try to login if not work follow bellow step change file permission

```
chmod go-rw privatekey.pem
```

```
chmod 400 <private-key-filename>.pem
```


## Steps For macOS .pem to .ppk

```
puttygen testkey1.pem -o testkey1.ppk
```

[Link stackoverflow ](https://stackoverflow.com/questions/37286791/convert-pem-to-ppk-on-macos)

[Link codeblocq ](https://www.codeblocq.com/2016/05/Convert-a-putty-ppk-key-to-a-pem-file-on-OSX/)

Both MacPorts and Homebrew are useful tools for managing software on a Mac, and they offer different sets of software packages and libraries. Users can choose which package management system to use based on their needs and preferences
