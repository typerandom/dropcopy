dropcopy
========

Upload a file directly to your dropbox in one line. Installs using APT (N/A yet).

=======================

Copy a file to the root directory in your Dropbox. Will prompt for username and password.

    dropcopy [path of file to copy]
    
=======================

Copy a file to the root directory of your Dropbox. Will prompt for username and password.

    dropcopy [path of file to copy]
    
=======================

Copy a file to a specific directory in your Dropbox. Will prompt for username and password.

    dropcopy -src [path of file to copy] -dst [dropbox path]
    
=======================

Copy a file to a specific directory in your Dropbox. Creating missing directories. Will prompt for username and password.

    dropcopy -src [path of file to copy] -dst [dropbox path] --force
    
=======================

Copy a file to the root directory of your Dropbox. Explicitly stating username and password (not recommended since it shows up in history).

    dropcopy -usr [dropbox username] -psw [dropbox password] -src [path of file to copy]
    
=======================

Copy a file to the root directory of your Dropbox. Loading username and password from a config file.

    dropcopy -conf /etc/dropcopy/auth.conf -src [path of file to copy]