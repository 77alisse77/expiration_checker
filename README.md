

# Root Key checker

## Intro

TAC engineers need to installl RootPatch to perform operations with root privileges on ISE nodes. Prior to the installation of RootPatch, we need to install a RootKey bundle that will install local developer public keys that can be used to verify the signature of the RootPatch bundle.

For security reasons, RootKey bundle expires after a fixed period of time, and there is no trivial way to know if a specific RootKey bundle has expired or not. The only option is to try and install it. In case it has already expired, it will throw an error and the intallation won't be completed. 

## RootKey bundle expires

For security reasons, RootKey bundle expires after a fixed period of time, and there is no trivial way to know if a specific RootKey bundle has expired or not. The only option is to try and install it. In case it has already expired, it will throw an error and the intallation won't be completed. 

## How to quickly check if a RootKey has expired
 
Prerequisites:
- Python installed on your computer. You can get it from https://www.python.org/downloads/. I'm using python 3.6
 
Procedure:
- Download the script from my repository (http://gitlab.cisco.com/aligarci/root_key.git) and place it in the same folder as your RootKey-appbundle-1.0-x86_64.tar.gz. 
- Execute the script, a message will be shown on console:

![alt text](https://techzone.cisco.com/t5/image/serverpage/image-id/146656i9EB2CD2E0DD37A30/image-size/large?v=1.0&px=800 "RootKey checker execution example")