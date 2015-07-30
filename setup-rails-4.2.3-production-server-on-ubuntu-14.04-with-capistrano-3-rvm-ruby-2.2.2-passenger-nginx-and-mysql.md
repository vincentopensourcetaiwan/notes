# environment
    ubuntu 14.04 64 bit
    rvm
    ruby 2.2.2p95
    rail 4.2.3
    passenger
    nginx
    mysql
    capistrano 3
    
# steps
### copy your LOCAL public key to the root user on the server (replace 0.0.0.0)
##### on your workstation

    ssh-copy-id root@0.0.0.0
    
type yes

enter password

### now you can login without password (replace 0.0.0.0)
##### on your workstation

    ssh root@0.0.0.0
    
### update packages
##### on your server

    aptitude update
    aptitude safe-upgrade
    
### add another user
##### on your server
       
    adduser creston
    
enter password
    
enter password again
    
enter to pass full name question
    
enter to pass room number question

enter to pass work phone question

enter to pass home phone question

enter to pass other question

enter to confirm the information


### add user to group sudo so that user can sudo all commands
##### on your server

    adduser creston sudo
    
### reboot system in case any installed patches require it
##### on your server

    reboot



    
    
    
# references
https://www.youtube.com/watch?v=WBPV4vjzcjQ&feature=youtu.be&a
https://gorails.com/deploy/ubuntu/14.04
https://www.youtube.com/watch?v=bhDUaxEC9oc
http://www.rubytreesoftware.com/resources/securely-setup-ubuntu-1404-server