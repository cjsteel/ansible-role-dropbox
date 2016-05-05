https://www.dropbox.com/download?dl=packages/ubuntu/dropbox_2015.10.28_amd64.deb

ansible apt requires

        python-apt
        aptitude

- apt: name=foo cache_valid_time=86400 update_cache=yes

https://github.com/jdauphant/ansible-role-dropbox.git

restart nautilus
install python-gpgme in order to verify signatures.

## Dropbox, where is the email address and password saved

The email address is in a file called config.db, which is in a folder called .dropbox in your home folder. It's an sqlite file, not a text file, so you can't just view it in gedit. Go to terminal and type:
    Code:

    sudo apt-get install sqlitebrowser

    Then open up sqlitebrowser and click File > Open Database. Navigate to the config.db file, and open it. Then click on "Browse Data" and scroll down. Near the bottom, it says email on the left, and your email address on the right. 


