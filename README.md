# Authorized Keys

Repository to store a list of my devices ssh keys. Together with helpers for adding new devices and installing these to new machines.

Im also including plain bash and cmd lines for installing this repository to any system that has access to the internet for easier one line copy paste deployment.

## Installing on Windows

curl https://raw.githubusercontent.com/JBDCE/authorizedkeys/refs/heads/main/authorized_keys >> %userprofile%\.ssh\authorized_keys

## Installing on Linux

curl https://raw.githubusercontent.com/JBDCE/authorizedkeys/refs/heads/main/authorized_keys >> ~\.ssh\authorized_keys


## Caveats and unsolved problems

Currently there are no countermeasures for adding a key twice. This is not necessarily a problem as sshd is not complaining but it might cause issues in the future. At which point a duplicate cleanup script should be added.
