# homebrew-paritytech
Homebrew Tap for paritytech.

### Getting Homebrew

Homebrew is the missing package manager for OSX. You can find installation instructions at www.brew.sh. Alternatively open your terminal and type in:

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### Adding Parity to your list of Homebrew 'kegs'

Open your terminal and enter:

```
brew tap paritytech/paritytech
```

### Installing Parity

If you wish to download and install the latest **stable** version of Parity, open your terminal and enter:

```
brew install parity --stable
```

If you would prefer to use the latest **beta** release, open your terminal and enter:

```
brew install parity
```

If you would prefer to use the latest **develop** release, open your terminal and enter:

```
brew install parity --master
```

In order to update Parity to the latest version use:

```
brew update && brew upgrade parity
```

and

```
brew reinstall parity
```
### Mac OSX Bug Fixes
If you are encountering permission or "Empty Installation" errors when attempting to execute the "parity" command in your terminal using Mac OSX, please follow these instructions: 

Open Users/your.username/.bash_profile, by using the following command in the terminal:

```
nano .bash_profile
```

Add the following line within the file via the terminal:

```
export PATH=/Applications/Parity\ Ethereum.app/Contents/MacOS:$PATH
```

Once you’ve copy and pasted the above line, press “control x” and then press “Y” to save the changes. Then press “Enter.” Restart terminal, (no need to restart your mac). Use the following command in the terminal:

```
parity
```

It should work now! Let us know if you have any issues and we can solve them together!
