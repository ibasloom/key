# convert .pem 2 .ppk | .ppk 2 .pem | macOS

## To convert a .pem file to a .ppk file on macOS, you can use the "puttygen" utility which is part of the PuTTY package. Here are the steps to follow:

### Step 1: Install PuTTY on your Mac using either of the following commands in Terminal:
------------

Using Homebrew:

```
brew install putty
```

Using MacPorts:

```
sudo port install putty
```

### Step 2: Open Terminal and navigate to the directory where your .pem file is located. Then, run the following command to convert the .pem file to .ppk format:
------------

```
puttygen your_key.pem -o your_key.ppk
```

This command will create a new .ppk file in the same directory as your .pem file. You can now use the .ppk file to connect to your server using SSH.

If you need to convert a .ppk file back to .pem format, you can use the following command:

```
puttygen your_key.ppk -O private-openssh -o your_key.pem
```

Note that you may need to change the file permissions on your key file using the "chmod" command before you can use it to connect to your server. To do this, run the following command:

```
chmod 400 your_key.pem
```

That's it! You should now be able to connect to your server using your converted key file.
