# LinuxShell_ssh

* telnet in secure way

        ssh -R [port of local host]:[remote host name or its IP addr]:[port of remote host]

        ssh -p [port of remote host]

        ssh -l [loggin_account]

        ssh -i [identify info]
        // check version,
        // if version is 1, then private key is in path of .ssh/identify
        // if 2, then .ssh/id_rsa and .ssh/id_dsa

 * Check key is exist or not
 
         ls -al ~/.ssh
 
      https://help.github.com/en/github/authenticating-to-github/checking-for-existing-ssh-keys
 
 * Generate key if not exist
 
      https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
  
  
    
    
   
