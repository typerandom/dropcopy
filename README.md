dropcopy
========

Upload a file directly to your dropbox in one line. Installs using APT (N/A yet).

## Install (not available yet!)

    sudo apt-get install dropcopy

## Usage

=======================

##### Copy a file to the root directory in your Dropbox. Will prompt for username and password.

    dropcopy [path of file to copy]
    
=======================

##### Copy a file to a specific directory in your Dropbox. Will prompt for username and password.

    dropcopy -src [path of file to copy] -dst [dropbox path]
    
=======================

##### Copy a file to a specific directory in your Dropbox. Creating missing directories. Will prompt for username and password.

    dropcopy -src [path of file to copy] -dst [dropbox path] --force
    
=======================

##### Copy a file to the root directory of your Dropbox. Explicitly stating username and password (not recommended since it shows up in history).

    dropcopy -usr [dropbox username] -psw [dropbox password] -src [path of file to copy]
    
=======================

##### Copy a file to the root directory of your Dropbox. Loading username and password from a config file.

    dropcopy -conf [path of config file] -src [path of file to copy]

=======================

## Examples

    dropcopy ~/awesome-file-in-the-house.zip

=======================

    dropcopy -src ~/filez/awezum-file.txt -dst /awezum-file123.txt
    
=======================

    dropcopy -src ~/filez/awezum-file.txt -dst /my-dropbox-textfiles/that_i_like/super_awesome/awezum-file123.txt --force

=======================

    dropcopy -usr catsnapper123 -psw OHMAHSECRETPSW999 -src ~/awesome-file.zip

=======================

    dropcopy -conf /etc/dropcopy/auth.conf -src ~/awesome-file.zip

=======================